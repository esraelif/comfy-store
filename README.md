![](https://github.com/esraelif/comfy-store/blob/main/src/assets/comfy.gif)

#Step (1) - Setup
create vite project with tailwind

#Step (2) - Setup DaisyUI
add and configure daisyui to our project
add TailwindCSS Typography plugin

#Step (3) - Create All Pages
create pages directory
create all pages and export from index.js
About, Cart, Checkout, Error, HomeLayout, Landing, Login, Orders, Products, Register, SingleProduct
import in app.jsx

#Step (4) - React Router
configure react router
setup initial route structure hint : look for nested UI (basically navbar)

#Step (5) - Error Page
complete error page
create two returns
first for 404 errors
second for all other errors
log the error
add option to navigate home

#Step (6) - Input Field Component
create components folder with index.js
in daisyui
find Text input component
more specifically "With form-control and labels"
set it as component (in my case FormInput.jsx)
decide on props
export from index.js
test in login
#Step (7) - Login Page Structure
setup structure for login page (use complete project as reference)
check for loading state and disable submit button
setup submit button in a separate component
add loading spinner

#Step (8) - Register Page Structure
setup structure for register page (use complete project as reference)

#Step (9) - Custom Class
create custom class
align content
add to HomeLayout Outlet component

#Step (10) - Header Component
setup and render header component in HomeLayout
add two links - Login and Register

#Step(11) - Navbar Structure
create components/Navbar.jsx
setup initial structure
use Daisy navbar component
"# responsive (dropdown menu on small screen, center menu on large screen)"
import icons from react-icons
render in HomeLayout.jsx

#Step (12) - NavLinks
create NavLinks component
setup an array of links
iterate over and setup return

#Step (13) - Toggle Component
add daisyui swap component

#Step(14) - Set Themes
add few themes from daisyui
test in index.html

#Step(15) - Change Theme
change theme with toggle component

#Step(16) - About Page
setup about page

#Step(17) - Hero Component
setup hero component in landing page

#Step(18) - Axios Custom Instance
explore api
API DOCS
create utils/index.js
setup custom axios instance
figure out the base url
setup thunder client (optional)

#Step(19) - Landing Loader
setup ErrorElement
add to Loading Page
setup a loader
fetch only featured products
return products

#Step(20) - Featured Products
create FeaturedProducts, SectionTitle and ProductsGrid components
render SectionTitle and ProductsGrid in FeaturedProducts
setup SectionTitle
in ProductsGrid access and render products from loader

#Step (21) - Format Price
payment providers need in smallest unit
in this case cents
in utils setup a function to format price
utilize in ProductsGrid

#Step(22) - Single Product
complete in multiple steps
fetch and render single product
don't forget about the colors and amount options
extra credit - set amount options dynamically

#Step(23) - Products Page (Setup)
create following components and render in products page
Filters
ProductsContainer
PaginationContainer
in products page loader fetch all products

#Step(24) - Products Container
create ProductsList and render products in one column
setup header (with total jobs and toggle buttons)
toggle between ProductsGrid and ProductsList

#Step(25) - Filters (Search Input)
add size to prop FormInput.jsx
render search input, submit button and reset button
setup input for select input
render for categories, companies and order
companies and categories values are located in meta
create range input (hint: you will need local state)
create checkbox input

#Step(26) - Global Loading
create loading component
check for loading state in HomeLayout
toggle between loading and

#Step(30) - Setup Params
explore how to filter products API DOCS
test in Thunder Client
access params in loader
use params in customFetch
pass params down
use params as default values (price in FormRange)
setup reset button#step(31) - Pagination
explore how to paginate
test in Thunder Client
access meta
display next, prev and page buttons
add page value to query params

#Step(31) - Pagination
explore how to paginate
test in Thunder Client
access meta
display next, prev and page buttons
add page value to query params

#Step (32) - Setup RTK and react-toastify
create features/cart/cartSlice.js
setup default state (README) and reducers
export actions and cartSlice.reducer
create store.js and add cartSlice
setup RTK and react-toastify in main.jsx

#Step (33) - Add Product
import and dispatch addItem action
add item to cart in SingleProduct page
display cartItems in Navbar
setup addItem functionality
refactor addItem and get default state from local storage
try to setup reducers for clear cart, remove item and edit item
create CartItemsList, CartTotals, CartItem components
export CartItemsList, CartTotals in components/index.js
setup two column layout in cart page
setup cart totals component
iterate over cartItems and return CartItem
in CartItem display values and implement remove,edit functionality

#Setup (40) - Setup User Slice
setup user slice
add to store
setup logout reducer
access user in Header, NavLinks and Cart Page
API DOCS
docs - register request
test in Thunder Client
setup action in Register
add action to Register route in App.jsx
