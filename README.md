# Exploratory_Data_Analysis
"On my first day practicing EDA (Exploratory Data Analysis) in data science, I found myself in an essential data science repository. Here, raw data is meticulously transformed into clean, analytical datasets, setting the stage for a transformative journey in the world of data science. With enthusiasm and curiosity, I dove into the data, ready to apply machine learning algorithms to build and refine data models. This marked a significant and progressive step in my data science journey, where I eagerly embraced the opportunity to explore, analyze, and draw insights from the wealth of information at my fingertips.

However, it wasn't all smooth sailing on my first day. I encountered my fair share of challenges and, in the spirit of transparency, documented the errors I faced in this README file. These errors are a testament to the learning process, and I am committed to overcoming them as I continue to grow in the field of data science."

ERROR I FACED-

1. i input that command "Sales=pd.read_csv("C:\Users\Dell\Desktop\75 Day\Diwali Sales Data.csv" , encoding='unicode_escape')" and i get this error " Cell In[13], line 1
    Sales=pd.read_csv("C:\Users\Dell\Desktop\75 Day\Diwali Sales Data.csv" , encoding='unicode_escape')
                                                                           ^
SyntaxError: (unicode error) 'unicodeescape' codec can't decode bytes in position 2-3: truncated \UXXXXXXXX escape"

REASON- The error you're encountering is due to the use of backslashes in the file path. In Python, backslashes are used as escape characters, and when you use them in a string, like a file path, you may encounter this error.

SOLUTION- 
1. Use Double Backslashes: You can escape the backslashes by using double backslashes in your file path:
Sales = pd.read_csv("C:\\Users\\Dell\\Desktop\\75 Day\\Diwali Sales Data.csv", encoding='unicode_escape')

2. Use a Raw String:
You can also use a raw string by prefixing the string with 'r'. This will treat the string as a raw string and won't interpret escape characters:
Sales = pd.read_csv(r"C:\Users\Dell\Desktop\75 Day\Diwali Sales Data.csv", encoding='unicode_escape')

