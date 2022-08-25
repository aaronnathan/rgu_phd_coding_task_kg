# Knowledeg Grapth Technical Interview question

## Task 1 (Knowledge extraction from text)
a) First of all, I created a function to import the content of the senteces.txt file into memory or my notebook.<br />
![image](https://user-images.githubusercontent.com/39290938/186638964-6db302fe-32d7-4623-9229-7d81eeff5883.png)<br />
This functon reads the content in the file specified and returns it.
<br /><br/>
b) Also, A function was created to extract all the entities in pasages.<br />![image](https://user-images.githubusercontent.com/39290938/186782469-f6cf9629-e217-403d-bfe6-582604139c80.png)
<br />
This function loops through each sentence and then extracts the entities and also calls the extract relations fuction to extract the relations in each sentence and return them accordingly. The entities are paired together but the relatons are seperated.<br/><br/>
I also created a fuction to extract all relationships from the sentences.This function works be first looking for the ROOT dependency. If the sentence has a ROOT dependency, it will go on to check if the ROOT is followed by an dobj. it will check till all the conditions in the specified rule are met. But if the matcher does not find the root dependency, it will go on to check whether the next item in the rule is available until all the conditions are checked. The image below shows the code snippet of the extract relationship function.<br/><br/>
![image](https://user-images.githubusercontent.com/39290938/186782623-6b0d31fa-60f2-4862-a254-c0fc70d26ac1.png)
<br/><br/>
c) I also created a function that takes the extrated entities and relationships as its parameters and then converts them into a datafram of three columns ['source','target','edge']. The source stores the subject and the target stores all the objects while the edge stores all the edges.
<br/>
![image](https://user-images.githubusercontent.com/39290938/186641172-42644c1c-2541-4632-a8f5-c5cd59f9e8fd.png)
<br/>
This method first extracts the entities and relations into a dictionary and the used pandas.Dataframe to convert the generated dictionary in to a dataframe. The image below shows how the dataframe looks like after it was generated.<br/>
![image](https://user-images.githubusercontent.com/39290938/186781838-623fb5ed-b326-4536-af67-03b75412aa20.png)
<br/><br/><br/>
## Task 2(Creation and visualisation of knowledge graph)
a) I made use of the NetworkX and matplotlib libray in generating the Knowlegde Grapth. The NetworkX library was used to draw and configure the Knowlegde graph. It was used to load the dataframe and then converted into the graph. matplotlib was then used to visualize the graph. The image below gives a snippet of the code used to perform this action<br/><br/>
![image](https://user-images.githubusercontent.com/39290938/186642708-bfffb9ae-b979-47be-a32c-e3c52a125981.png)
<br/><br/>
The image below shows how the Knowledge graph looked like after it was generated.<br/><br/> 
![image](https://user-images.githubusercontent.com/39290938/186782332-f7ce7b79-5f09-411d-a7a9-ff96373ba48f.png)







