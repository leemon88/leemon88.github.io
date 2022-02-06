import pandas as pd

data = pd.read_excel ("C:\\Users\\johns\\Downloads\Copy of Winter 9th grade Tournament Official Stats.xlsx")
print(data.head(28))

#create dataframe

#render dataframe as html
html = data.to_html()

#write html to file
text_file = open("index.html", "w")
text_file.write(html)
text_file.close()
