### Conceptual Exercise

Answer the following questions below:

- What is the purpose of the React Router?
   React Router, and dynamic, client-side routing, allows us to build a single-page web application with navigation without the page refreshing as the user navigates.
- What is a single page application?
Single Page Applications are a great tool for making incredibly engaging and unique experiences for your users.
- What are some differences between client side and server side routing?
The difference between this two routing have been stated above server sides needs to keep making requests to the server in order for the application to rerender, but client side does not need to keep make request to the server, it just does it once when the application is being loaded into the browser any other navigation or page change is just being rendered from the already saved application, so a client side application can still function without the internet as long as it has already being loaded in with the internet.
- What are two ways of handling redirects with React Router? When would you use each?
1. Import Redirect
Turns out, <Redirect /> is built into React Router DOM, so all you need to do is import it at the top of your file. If you haven’t already, you’ll need to install react-router-dom using npm. Once that’s ready to go, import redirect in the relevant file/component as such:
import { Redirect } from "react-router-dom";
2.Conditionally Render the Redirect Component
For this, you can use ternary operators or switch cases. To refresh on ternaries:
thingThatReturnsTrueOrFalse ? thingThatHappensIfTrue : thingIfFalse
You will need this ternary to sit somewhere in the rendered part of the component. I beat my head against a brick wall getting redirects to work before I realized this. It’s not enough to simply return a redirect somewhere in your code, it needs to actually render.
- What are two different ways to handle page-not-found user experiences using React Router? 
1.By using React Router’s <Switch /> and adding the NotFound component at the bottom of our <Route /> declarations we are able to ensure that the route only works when we hit an unregistered route.
2.Using a React RedirectRedirect the 404 Error Elsewhere
Correct the source link
Restore deleted pages
Ignore the not-found error

- How do you grab URL parameters from within a component using React Router?
To capture url parameters use window object. You can use "useLocation" from "react-router-dom" instead of window object to achieve same results.
- What is context in React? When would you use it?
React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props. In other words, React context allows us to share data (state) across our components more easily.
- Describe some differences between class-based components and function
  components in React.
  -A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element.	
  -A class component requires you to extend from React. Component and create a render function which returns a React element.
  -There is no render method used in functional components.
  -Class component must have the render() method returning HTML


- What are some of the problems that hooks were designed to solve?
 the use of hooks reduces the number of concepts needed in the development of React applications, so that we do not need to continuously switch between functions, classes, HOCs or elements to perform similar tasks; hooks offer us homogeneity in the ecosystem.