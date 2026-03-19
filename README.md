1.What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

ans: The difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll are given below:

getElementById-
(i)Finds ONE element only
(ii)Uses the element’s id
(iii)Fastest method

getElementsByClassName-
(i)Returns multiple elements
(ii)Uses class name
(iii)Gives a live collection (auto-updates if DOM changes)

querySelector-
(i)Returns only the FIRST match

querySelectorAll-
(i)Returns all matching elements
(ii)Gives a static NodeList 


2. How do you create and insert a new element into the DOM?
   
   ans:
    (i)Create the element
   const newDiv = document.createElement("div");
   (ii)Add content inside it
   newDiv.textContent = "Hello, I am new here!";
   (iii)Insert it into the DOM
   document.body.appendChild(newDiv);

   3. What is Event Bubbling? And how does it work?
      
      ans: Event Bubbling is a concept in JavaScript, where
      ->It starts from the clicked element
      ->Then moves up to its parent
      ->Then grandparent
      ->all the way up to document

      ex:
      <div id="parent">
      <button id="child">Click Me</button>
     </div>
     it works like->
     (i)The event first triggers on the <button> (child)
     (ii)Then it “bubbles up” to the <div> (parent)
     (iii)Then continues up to <body> → <html> → document

     4. What is Event Delegation in JavaScript? Why is it useful?
        ans:Instead of adding event listeners to many child elements,
           you add ONE event listener to their parent… and handle everything from there.
           It works because of event bubbling.

    it is useful,because-
   1.One listener instead of many
   2.Even if you add new buttons later, it still works
   3.Less repetition

   5. What is the difference between preventDefault() and stopPropagation() methods?
      ans:The difference between  preventDefault() and stopPropagation() methods are given below:

      event.preventDefault()-
      Stops the browser’s default behavior for an event.
     (i)Clicking a link → normally opens a URL
     (ii)Submitting a form → normally reloads the page

      event.stopPropagation()-
      Stops the event from bubbling up the DOM tree.
      
      











     












   
   
