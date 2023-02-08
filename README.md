# Yahoo 1-1 Interview Conducted by Kavitha Kamarasamy
### Interview Recording Link – [Click Here](https://wipro365-my.sharepoint.com/:v:/g/personal/ka20161415_wipro_com/ER0LKvpLFuNKopl440RN1D8B_E2-u_X5mrdp9U3bNtGjHQ)
##### Ishvinder Singh
##### [Ishvinder.singh2@wipro.com](ishvinder.singh2@wipro.com)
- ### [Test 1 Report](https://github.com/ishvinder9528/Yahoo-Assessment-Report/blob/main/Report_Front-End_Developer__React__Ishvinder_Singh_ishvinder.singh2_wipro.com.pdf)
- ### [Test 2 Report](https://github.com/ishvinder9528/Yahoo-Assessment-Report/blob/main/Report_Front-End_Developer_Test_2_ishvinder.singh2_wipro.com.pdf)
### Questions Asked in Interview
#### Can you Tell me about Yourself?
###### Yes, Good Evening, Kavitha, My Name Is Ishvinder Singh. I have Completed my Graduation in Computer Science Engineering from Moradabad Institute of Technology, Moradabad, Uttar Pradesh. And I joined Wipro in July,2022. Before Joined Wipro, I done certification in ‘Java Full Stack’ by StackRoute that was given by Wipro itself.
###### And Currently I’m Working as a Frontend Enginner. That’s it.
#### What is your Plus? What is Your Minus?
###### Umm.. Basically I’m Very dedicated to one thing, If you give me some Assignment/task or something. I can complete this and get the output at any cost.
#### Do you know what is TypeScript?
###### Yes, I know about TypeScript. Basically, it is the Strict Version of the JavaScript.
#### Difference between var and let?
###### Both are used for initializing the variable. But var are having the global scope, while on the other hand let have the block scope initializer.
#### What is Hoisitng?
###### Basically in the Java Script, we can use the variable before initializing it. That is Hoisting.
#### arr = [2,4,[1,2],7,9,10,[33,44,55],66] Convert it into single array/1-D array.
    arr= [2,4,[1,2],7,9,10,[33,44,55],66]
    console.log(arr.flat())
#### Difference between ‘==’ and ‘===’?
###### ‘==’ checks the value is same or not, while on the other hand ‘===’ checks there datatype too.
#### Make 3 Div, as div1 inside div2 and div2 inside div3. And when we click on Div3 alert box appear and says ‘I am div3. Style it by making the border different and setup their height and width and justify all in centre to each another’
    <div
        style={{
          backgroundColor: "blue",
          width: "200px",
          height: "200px",
          display: "flex",
          alignItems: "center",
          justifyContent: "center"
        }}
      >
        <p>Div1</p>
        <div
          style={{
            backgroundColor: "red",
            width: "100px",
            height: "100px",
            display: "flex",
            alignItems: "center",
            justifyContent: "center"
          }}
        >
          <p>Div2</p>
          <div
            onClick={() => {
              console.log("i am div 3");
            }}
            style={{
              backgroundColor: "black",
              color: "white",
              width: "50px",
              height: "50px",
              display: "flex",
              alignItems: "center",
              justifyContent: "center"
            }}
          >
            <p>Div3</p>
          </div>
        </div>
      </div>
#### Make an text box and a button. When we click on button the data on the textbox will appear downside of the box and make a todo app like this.
    import React, { useState } from "react";
    export const Todo = () => {
    const [list, setList] = useState([]);
    const [input, setInput] = useState("");
    const submitTodo = () => {
      console.log("Button works");
      setList([...list, input]);
      setInput("");
    };

    // Step 1 -  create textbox and button
    // step 2 -  make an empty list
    // step 3 -  make a function who take the data from the textbox
    //           and add it to list
    // step 4-   show the list data to the main page by using map func.
    return (
      <>
        <h1>Todo</h1>

        <input
          name="todos"
          id="todoInput"
          value={input}
          placeholder="enter todo"
          onChange={(e) => setInput(e.target.value)}
        />
        <button name="todos" type="submit" onClick={submitTodo}>
            Submit Todo
        </button>
        <h2>Todo list</h2>
        <ul>
          {list.map((t) => (
          <li>{t}</li>
          ))}
        </ul>
        </>
        );
        };
#### Tell me the pseudo code of what you going to done in this to-do app.
````
  Step 1 - create textbox and button
  Step 2 - make an empty list
  Step 3 - make a function who take the data from the textbox and add it to list
  Step 4-   show the list data to the main page by using map func.
````
#### Difference Between Arrow And simple Function?
###### Basic Difference is in the Arrow Function we don’t need to write the function and return syntax. And the second is they are considered as the variable.
