## Todo React Native

### Requirements

- [Design](react-native-assessment.sketch.pdf)
- Use @expo/react-native-action-sheet
- Use @react-navigation
- Use @reduxjs/toolkit
- Use Expo
- Use react-hook-form
- Use redux-persist
- Use typescript

#### Login

- If no name exists, a new account will be created
- If name exists, show all todos created by this account

#### Todo

- Click on todo will show action sheet, which has 4 actions - Complete, Edit, Delete and Cancel
- Reference design for completed todo UI
- Edit todo will navigate to a new screen which has the similar UI as add todo
- In Edit todo screen 1. add back button in the header 2. remove title `Add` 3. replace button `Add` with `Save` 4. do not show bottom tabs
- Edit todo has data prefilled
- Delete todo should ask user to confirm with an alert

#### Add

- Description, due and color are all required
- When click on `Add`, if any field is missing show a toast mentioning the missing fields, and the toast should disappear in 2 seconds
- Due must be a string following format `YYYY-MM-DD`, otherwise a toast with error message will show, and the toast should disappear in 2 seconds
- Selected color should have full opacity, others shouldn't
- Edit todo should also follow the above requirements
