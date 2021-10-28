# KD_Project<br />
Its requirede to have our Ontology loaded into GraphDB under the repository name "ogc"

# To enable the widgets in the notebook use cmd commands:<br />
- jupyter nbextension enable --py widgetsnbextension

# The functionalities of this Notebook are:<br />
-Showing Codon Distribution for a species using its SpeciesID with a custom Plot<br />
---> useage: get_codon_graph(SpeciesID)
  
-Showing Similarities between two Species using a cusotm Plot and overall Similarity<br />
---> useage: compare(SpeciesID1, SpeciesID2)
  
-Getting an organisms Lineage and its indices using the SpeciesID<br />
---> useage: get_lineage(SpeciesID)
  
#Automatic Querying and SPARQL-Query generator using a Form<br />
The last part of the Notebook contains a Form that lets a user Query for an organism in a very simple way.<br />
-> after the form is filled do not run the Cell again , otherwise it resets

How to use:<br />
-> Indicate how many statements the query should have (statement = (p,s,o))<br />
-> Indicate how many variables you want to query for

run the next cell<br />
-> Indicate if you want to count something and if yes what<br />
    ---> this is a dropdown menu where you can select any variable generated<br />
-> For each line indicate the Predicate, Subject and Object (the predicate stays the same for all lines)<br />
   ---> if you search for a lable the input is not case sensetive and accepts small errors

run next cell<br />
-> Indicate if there should be a limit for the output, if it stays 0 it wont be used as LIMIT<br />
-> Indicate if on which variable the output should be sorted and of which order

--> The query will return the results automatically once the next cell is run and the GraphDB repository has been set-up
