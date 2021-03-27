# Tableau-Prep-Project
Final Data Flow
Please refer to powerpoint file for project walk through
This project heavily emphasizes in utilizing basic features that Tableau Prep Software has to offer.
I was able to successfully create extract, slice and dice data in order to generalize relationship between rank with other data factors i.e. List, Author and Prices.
Let me explain my data flow and results more in detail.

![image](https://user-images.githubusercontent.com/75600348/112736653-96135f00-8f11-11eb-9ff1-2a6693a62e64.png)

In this screenshot we can see how there are more fields and less rows. Each field value is broken into several pieces such as Title, Author, Price, ISBN, Previous Ranks, Weeks on List. For Example: Look at Hardcover Fiction Field Value broken into pieces.
My project focuses on generalizing list of field values and creating results accordingly.

![image](https://user-images.githubusercontent.com/75600348/112736674-ae837980-8f11-11eb-8189-fa9333931aa4.png)

Original Data included massive monthly details of best sellers books based upon different genre-title, genre-author, genre-price, genre-ISBN, genre-Previous Rank, genre-Weeks on List
The goal of designing this data flow was to reduce the number of fields by organizing data in simple manner. 
My first step was to unionize all data from different dates of January.

![image](https://user-images.githubusercontent.com/75600348/112736686-cc50de80-8f11-11eb-9df8-81d61a561fee.png)

![image](https://user-images.githubusercontent.com/75600348/112736689-d1159280-8f11-11eb-8e1c-4d5ffb3ec93c.png)

![image](https://user-images.githubusercontent.com/75600348/112736693-d7a40a00-8f11-11eb-8f3b-48645cc6663a.png)

Data Pivoting
Data Pivoting is a crucial step in this steps as it helps pivoting data from columns  values to fields. 
In this flow once I unionized all excel data into one database. I did some neat and tidy up work to keep the data more consistent and organized.
Then I separated data based on one field factor i.e. Previous Rank, Weeks, ISBN, Author, Titles and Prices.
Lets look at it in more detail by focusing on Pivoting Results.
![image](https://user-images.githubusercontent.com/75600348/112736705-f0142480-8f11-11eb-8460-749f8d2ac505.png)
Pivoting Results
Lets focus on one field and that is Author. 
Here I separated Author and other relevant fields as one piece of data flow.
The data is CLEANED based on relevant fields to Author in this step. Week, Rank, Hardcover Fiction, Hardcover Nonfiction, Mass Market, Trade Paperback Nonfiction, Early & Middle, Young Adult.
Once data is organized it is then Pivoted in Columns to Rows mode. 

![image](https://user-images.githubusercontent.com/75600348/112736727-1afe7880-8f12-11eb-9ba1-7294da59dd8f.png)

The pivoting feature helped organize data by allowing to switch columns to rows which would simplify and differentiate data in terms of Week, List, Rank, Author.
Example: List of columns is field values now -  Hardcover Fiction, Hardcover Nonfiction, Mass Market, Trade Paperback Fiction, Trade Paperback Nonfiction, Early & Middle, Young Adult

![image](https://user-images.githubusercontent.com/75600348/112736738-3ff2eb80-8f12-11eb-8901-243c0930bf19.png)

Profile Pane: Here is look into profile pane of Author set results. 

![image](https://user-images.githubusercontent.com/75600348/112736746-4aad8080-8f12-11eb-919f-3bf3e0c1c8ff.png)

![image](https://user-images.githubusercontent.com/75600348/112736751-4ed99e00-8f12-11eb-84a1-6bb528f9bf82.png)

Data Join
Tableau Prep allows to join data through join clauses. I was able to join ISBN and Author sets which can be processed furthermore. 

![image](https://user-images.githubusercontent.com/75600348/112736768-703a8a00-8f12-11eb-93fb-9ec6b534ca41.png)

![image](https://user-images.githubusercontent.com/75600348/112736772-73ce1100-8f12-11eb-95de-052c11eabe72.png)

After applying necessary join clauses, the data just needed little tidying up i.e. field extraction and filtering.
The last step of flow is creating data output in .hyper format.

![image](https://user-images.githubusercontent.com/75600348/112736783-82b4c380-8f12-11eb-8654-eb125eac33d8.png)

Through simplification and data manipulation, I created 3 outputs with relevant data that can be analyzed through comparison of rank with other fields.
Outputs- Rank vs. Weeks on List, Rank vs. Author, Rank vs. Prices

![image](https://user-images.githubusercontent.com/75600348/112736794-919b7600-8f12-11eb-8864-aca1a86401d0.png)

![image](https://user-images.githubusercontent.com/75600348/112736795-94966680-8f12-11eb-9872-9194149d3c1d.png)

![image](https://user-images.githubusercontent.com/75600348/112736797-9829ed80-8f12-11eb-92b8-5db53fe9af9e.png)










