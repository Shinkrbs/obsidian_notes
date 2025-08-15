Tags: #React #Typescript

**React** is a JavaScript library for building user interfaces using individual pieces called components.

---

# How to Setup React with Vite

Tags: #Vite #Sertup

```terminal
npm create vite@latest
// select needed information
cd to_project_directory
npm install
npm run dev // to test if setup is done correctly
```

---
# Difference between Library and Framework

Tags: #Library #Framework 

## Library

A tool that provides a specific functionality

## Framework

A set of tools and guidelines for building applications.

---
# Fragment

Tags: #Fragment

A **Fragment** is an invisible container that lets you group multiple elements without adding extra HTML to the DOM.

```typescript
function ListGroup() {
return (
	<> {/* Means automatic fragment*/}
		<h1>List</h1>
		<ul className="list-group">
		<li className="list-group-item">An item</li>
		<li className="list-group-item">A second item</li>
		<li className="list-group-item">A third item</li>
		<li className="list-group-item">A fourth item</li>
		<li className="list-group-item">And a fifth one</li>
		</ul>
		</>
	);
}
export default ListGroup;
```

```typescript
function ListGroup() {
return (
	<Fragment> {/* Means automatic fragment*/}
		<h1>List</h1>
		<ul className="list-group">
		<li className="list-group-item">An item</li>
		<li className="list-group-item">A second item</li>
		<li className="list-group-item">A third item</li>
		<li className="list-group-item">A fourth item</li>
		<li className="list-group-item">And a fifth one</li>
		</ul>
		</Fragment>
	);
}
export default ListGroup;
```

---
# React Basic Information

Tags: #Components

## Components

A component is just a javaScript function that returns **JSX**. JSX looks like HTML  but it runs inside javaScript.

```JavaScript
function Hello() {
	return <h1>Hello!</h1>;
}
// Usage
<Hello />
```

## Props

Make dynamic components. **Props** which are basically just inputs. Just like when a function takes an argument, components takes props.

```TypeScript
export interface PersonProp{
	name: string;
	age: number;
	isMarried: boolean;
}

export const Person = (props: PersonProp) => {
	return (
		<div>
			<p>Name: {props.name}</p>
			<p>Age: {props.age}</p>
			<p>Marital Status: {props.isMarried ? "Married" : "Single"}</p> 
		</div>
	);
};

// Usage
function App() {
	return (
		<>
			<Person name={"Pedro"} age={22} isMarried={false} />{" "}
			<Person name={"Collin"} age={19} isMarried={true} />{" "}
		</>
	);
}

export default App;
```