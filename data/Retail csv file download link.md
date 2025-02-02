# Method 1
### The Download Link of Raw retail.csv
 https://archive.ics.uci.edu/dataset/352/online+retail

# Method 2
### Direct Download to your Python Envioronment
data_url = 'https://archive.ics.uci.edu/static/public/352/data.csv'

retail = pd.read_csv(data_url)

print(retail.shape)

print(retail.columns)

# Method 3
!pip install ucimlrepo


### In the second cell
from ucimlrepo import fetch_ucirepo 
  
### fetch dataset 
online_retail = fetch_ucirepo(id=352) 
  
### data (as pandas dataframes) 
X = online_retail.data.features 
y = online_retail.data.targets 
  
### metadata 
print(online_retail.metadata) 
  
### variable information 
print(online_retail.variables) 

