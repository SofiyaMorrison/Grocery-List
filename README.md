<!-- NAME OF THE PROJECT -->
   # Grocery List
   
   <!-- ABOUT THE PROJECT -->
   ## About The Project

This project helps people to create a Grocery List and then remove their iteams from the list with very easy way doing that. 

No ink or paper needed.

### Getting Started

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### How to use the App.

1. After you opened a Grocery List App via [http://localhost:3000](http://localhost:3000), you can type in your grocery iteams in open input window that says "What do you want to buy today? :
   
   ####
 **```
      <input type="text"
      ```**
   
   **```
      placeholder="What do you want to buy today?"
      ```**

 **```
      onChange={(e)=>{this.onChangeEvent(e.target.value)}}
      ```**

 **```
      value = {this.state.userInput}/>
       ```**
       
 ##### **Note: file - GroceryList.js.**

2. Then Add your iteam in a list by pressing **ADD** button,
   ####
 **```
       <button onClick={()=>this.addItem(this.state.userInput)} className="add">
      ```**

 **```
       Add
     ```**
     
 **```
       </button>
       ```** 
   
   ,*OR* use button **Enter** on a keyboard.
   
   #####     **Note: file - GroceryList.js.**

 3. If you bought an iteam from your list you can cross it out by clicking on that grocery iteam and crossed red line will pop up on it :
    ####
    **```
                <ul>
           ```**

     **```
                {this.state.groceryList.map((item,index)=>(
          ```**
    
     **```
                    <li onClick={this.crossedWord}
          ```**
     
     **```
                     key = {index}> 💎{item}
          ```**
    
     **```
                     </li>
         ```**
    
    **```
                ))}
          ```**
    
    **```
               </ul>
            ```**
            
   ##### **Note: file - GroceryList.js.**
   
    And
    
 ####
 **```
            .crossed{
            ```**

   **```
             text-decoration: line-through 2px red;
              ```**
              
 **```
             background-color: #f0f0f0;
              }
             ```**
             
   ##### **Note: file - App.css.**
    
 4. If you would like to remove all iteams from your list, then click on button **DELETE** :
       ####
 **```
        <button onClick={()=>this.deleteItem()} className="delete">
       ```**
       
   **```
                    Delete
                    ```**
                    
 **```
                </button>
                ```**
                
 ##### **Note: file - GroceryList.js.**
       
  

### Built With

  #### 
   * [React](https://react.dev/)
   * CSS
   * HTML
 





