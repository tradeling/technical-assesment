## Simple Ecommerce App
> Build a Simple ecommerce app

The core task is to build a simple commerce app with three main screens:
* Home, Display a list of products, You can use multiple widgets to display products by categories
* Product Detail, Display main product information, Including Product photos , Price, Description, etc
* Profile, User Profile where user can toggle RTL, Enable notification, Enable location, Manage Addresses
* Cart, Basic Cart implementation. With features like add to cart, edit cart. No need for APIs or checkout page

### Foundation
- [ ] First time app open, ask user to allow notification
- [ ] Build 2 bottom tabs - home & profile
- [ ] Build api loader
- [ ] Build api error toast
- [ ] Build api empty response screen

### Home
- [ ] Build product listing screen
- [ ] Build pull to refresh
- [ ] Build infinite scrolling with loading more products

### Product detail
- [ ] Build product detail screen
- [ ] Open a deeplink from outside the app will open the app and redirect user to product detail screen

### Cart
- [ ] Implement Add to cart
- [ ] Build Cart detail screen

### Profile
- [ ] There are 4 buttons in profile screen - toggle rtl & enable notification & enable location & addresses

### Toggle rtl
- [ ] Toggle rtl button will change the whole app layout without re-start the app

### Enable notification & location
- [ ] Enable notification and location button will lead user to the permission setting screen in your phone

### Addresses
- [ ] Addresses button will lead to address listing screen with add address button
- [ ] Add address button will lead to map view screen, and ask user to allow location fist time
- [ ] In map view screen, default address will be user's current location, and user can change location through a pin which is in the center of the screen
- [ ] After user add address in map view, the address will be reflected in address listing screen

### Stack
- [ ] Use @react-navigation
- [ ] Use @reduxjs/toolkit
- [ ] Use Expo
- [ ] Use typescript
- [ ] Use https://fakestoreapi.com/
