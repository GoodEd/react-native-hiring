# Doubt Tagging/Solving App:


### Flow

1. User Logins
2. Chooses Answer Doubts option. 
3. Sees a list of doubts. Spec: 
   * Doubts list is divided into 2 sections: 
      * High Priority - doubts that do not have an answer since 1 hour. 
      * All - rest of the doubts. 
4. User clicks on a particular doubt that they want to solve. 
5. After selecting the doubt they want to solve, they are provided with the option to check the details for the doubt. Spec: 
   * Subject (required) - to which subject this doubt belongs. Will be autofilled by server. 
      * In case the server doesn't have details for the doubt's subject, the user can tap on the subject field and the dropdown will ping the server to populate all subjects.
      * Use Physics, Chemistry, Biology as fields to populate. 
   * Chapter (required) - to which chapter this doubt belongs. Will be autofilled by server.
     * Spec remains same as mentioned in subject in case the doubt doesn't have details for the chapter. 
     * Use 2 chapters per subject. 
        * Names can be random. 
        * Informed Dropdown: The idea is when the user selects Physics in subject dropdown -> the chapter dropdown pings the server to get only the physics chapters. 
   * Topic (required) - to which topic this doubt belongs. 
     * Spec remains same if topic is not filled. 
     * Use 2 topic per chapter per subject. 
       * Names can be random. 
       * Informed Dropdown
   * Type of Doubt (required). Spec: 
      * the default options are good and bad. User can select between those two. 
   * Level of Difficulty (required)- the default options are high, medium, low. User can select between the three. 
   
6. After filling all the required options above, the user can now add solution to the doubt by clicking on add answer option which only becomes a button unless you have filled all required options. 
7. After clicking all add answer button -> user is now shown the view to add answer. Spec:
   * User can upload answer in three formats: 
     * Voice recording
     * Image
     * Text
     
8. After submitting, the user should be able to edit and delete their answer. 


## Screens

### 1. Login Screen: 
![Home Screen](https://github.com/GoodEd/react-native-hiring/blob/master/screens/Home.png)

### 2. Choose Option Screen:
![Options](https://github.com/GoodEd/react-native-hiring/blob/master/screens/Options.png)

### 3. List of Doubts
![List of Doubts](https://github.com/GoodEd/react-native-hiring/blob/master/screens/Answer%20Doubts.png)

### 4. Particular Doubt View
![Particular Doubt View](https://github.com/GoodEd/react-native-hiring/blob/master/screens/Answer%20Doubt%20-%3E%20Good%20Doubt%20Flow%20-%3E%20Home%20Screen.png)

### 5. Answer Doubt 
![Answer Doubt](https://github.com/GoodEd/react-native-hiring/blob/master/screens/Answer%20Doubt%20-%3E%20Good%20Doubt%20Flow%20-%3E%20Answer%20Mode.png)

### 6. Answered Doubt with voice recording
![Voice Recording](https://github.com/GoodEd/react-native-hiring/blob/master/screens/Answer%20Doubt%20-%3E%20Good%20Doubt%20Flow%20-%3E%20Answer%20Doubt%20-%3E%20Voice%20Recording.png)

### 7. Submitted answer - option to edit and delete
![Submit Answer](https://github.com/GoodEd/react-native-hiring/blob/master/screens/Answer%20Doubt.png)
