# KeeperApp
https://unx-robert.github.io/Keeper

## Components
- App.jsx component that renders all the components together
- Header.jsx component that renders a header element to show the Keeper app name in an h1
- Footer.jsx component that renders a footer element to show a copyright message in a p dynamically updated year
- Note.jsx component to show a div element with a h1 for a title and a p for the content
- CreateArea.jsx component to show a form element with a input for a title and a textarea>for the content of the note and a button for submitting the note
 
## Features
 - render all the notes as separate note components
 - add note functionality
 - delete note functionality
 - expanding features for input using conditional rendering
 - used some prebuild components

## How
- to keep track of the notes added i used the useState hook, the notes variable is an array of objects that have a title and a content as properties
- for the add functionality i used the useState hook to keep track of the changes of the input and textarea elements, and when the button add is pressed, the note is saved and sent to the addNote function on the App.jsx component that saves it in the notes array
- for the delete functionality i added a onClick event on the delete button that sent back the id of the note to be deleted to the deleteNote function on the App.jsx component that filters the note array and return only the objects with a different id
- for the expanding feature i used the useState hook to check when the textarea is pressed and the ternary operatory: if is pressed than render the input and the button and also make the textarea 3 lines else render only the textarea with 1 line
