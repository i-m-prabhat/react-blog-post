# React Blog Post

This is a React blog page that takes input as title and description and stores the title in a slug and stores it in a JSON-server with the current date, and shows the blog's title and date in another component. When you click on the blog title, it shows the full blog, and the title slug shows in the URL

## Code Explanation

The above code is a React application that creates and displays blogs. The application has two components: BlogPage and BlogDetail.

BlogPage component:

It is the main component that displays a form to add new blogs and a list of existing blogs.
It uses the useState hook to manage the state of the title and description of the new blog being added.
It uses the useEffect hook to fetch a list of existing blogs from the JSON server and store it in the component's state.
The component also contains a handleSubmit function that is called when the form is submitted. This function uses axios to send a POST request to the JSON server to add a new blog. The new blog data includes the title, description, current date, and a title slug (the title in lowercase with spaces replaced by hyphens).
The component displays a form to add new blogs and a list of existing blogs. The list of blogs includes the title and date of each blog and uses a Link component from react-router-dom to create a link to the full blog detail.
BlogDetail component:

This component displays the full detail of a single blog.
It uses the useParams hook from react-router-dom to get the title slug of the blog from the URL.
It uses the useEffect hook to fetch the detail of the blog from the JSON server based on the title slug.
The component displays the title, description, and date of the blog.
The App component is the root component of the application and it uses Route components from react-router-dom to define the routing of the application. It has two routes: the main route (/) that displays the BlogPage component, and the blog detail route (/blogs/:titleSlug) that displays the BlogDetail component.

The JSON server is used to store and retrieve the blogs. The application uses axios to send HTTP requests to the JSON server to add and retrieve blogs.

### This Blog post project is created by Prabhat
