# Knowledeg Grapth Technical Interview question

## Task 1 (Knowledge extraction from text)
a) First of all, I created a function to import the content of the senteces.txt file into memory or my notebook.<br />
![image](https://user-images.githubusercontent.com/39290938/186638964-6db302fe-32d7-4623-9229-7d81eeff5883.png)<br />
This functon reads the content in the file specified and returns it.
<br /><br/>
b) Also, A function was created to extract all the entities in pasages.<br />![image](https://user-images.githubusercontent.com/39290938/186639639-a8db6ff0-71a4-4ac6-911e-2589f029b936.png)<br />
This function loops through each sentence and then extracts the entities and relations and return the accordingly. The entities are paired together but the relatons are seperated.<br/><br/>
c) I also created a function that takes the extrated entities and relationships as its parameters and then converts them into a datafram of three columns ['source','target','edge']. The source stores the subject and the target stores all the objects while the edge stores all the edges.
<br/>
![image](https://user-images.githubusercontent.com/39290938/186641172-42644c1c-2541-4632-a8f5-c5cd59f9e8fd.png)
<br/>
This method first extracts the entities and relations into a dictionary and the used pandas.Dataframe to convert the generated dictionary in to a dataframe. The image below shows how the dataframe looks like after it was generated.<br/>
![image](https://user-images.githubusercontent.com/39290938/186642028-69278096-ee51-4bfb-b5ed-107fd650be37.png)
<br/><br/><br/>
## Task 2(Creation and visualisation of knowledge graph)
a) I made use of the NetworkX and matplotlib libray in generating the Knowlegde Grapth. The NetworkX library was used to draw and configure the Knowlegde graph. It was used to load the dataframe and then converted into the graph. matplotlib was then used to visualize the graph. The image below gives a snippet of the code used to perform this action<br/><br/>
![image](https://user-images.githubusercontent.com/39290938/186642708-bfffb9ae-b979-47be-a32c-e3c52a125981.png)
<br/><br/>
The image below shows how the Knowledge graph looked like after it was generated.<br/><br/> 
![image](https://user-images.githubusercontent.com/39290938/186643812-a4ff41b6-12d6-4745-ac77-d06724a35ea8.png)







