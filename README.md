Chef's Menu App - React Native with Expo

A mobile application built with React Native and Expo that allows customers to view a chef's menu and prices, while enabling the chef to login and manage menu items.


Features

For Customers (Client View)
• Browse menu items with prices and descriptions
• Filter menu items by category (Appetizers, Main Course, Desserts, Beverages)
• View detailed information about each menu item
• View item availability status
• Add items to order (simulated)
• Favorite items (simulated)


For Chefs (Management View)
• Secure login authentication
• Complete dashboard for menu management
• Add new menu items
• Edit existing menu items
• Delete menu items
• Toggle item availability
• Manage prices and descriptions
• Category-based organization


Technical Stack
• **React Native** with **Expo Go** compatibility
• **React Navigation** for navigation between screens
• **AsyncStorage** for local data persistence
• **Vector Icons** for UI icons
• **React Hooks** for state management


Installation & Setup

Prerequisites
• Node.js (version 14 or higher)
• Expo CLI: `npm install -g expo-cli`
• Expo Go app on your mobile device


Steps
1. **Install Dependencies**
```bash
npm install
```

2. **Start Development Server**
```bash
npm start
```

3. **Run on Device**
- Download Expo Go app on your iOS or Android device
- Scan the QR code shown in the terminal
- The app will load on your device


Demo Credentials

For testing the chef dashboard:
• **Username:** `chef`
• **Password:** `chef123`


App Structure

src/
\u251c\u2500\u2500 screens/
\u2502   \u251c\u2500\u2500 LoginScreen.js          # Chef authentication
\u2502   \u251c\u2500\u2500 MenuListScreen.js       # Menu browsing (customer view)
\u2502   \u251c\u2500\u2500 MenuDetailScreen.js     # Detailed item view
\u2502   \u251c\u2500\u2500 ChefDashboardScreen.js  # Chef management dashboard
\u2502   \u2514\u2500\u2500 EditMenuItemScreen.js   # Add/Edit menu items
App.js                          # Main app component with navigation


Key Features Explained

Authentication
• Simple login system for chefs
• Customers can continue without login
• Persistent authentication using AsyncStorage


Menu Management
• Full CRUD operations on menu items
• Category-based organization
• Availability status management
• Price and description editing


User Experience
• Clean, intuitive interface
• Loading states and error handling
• Responsive design for various screen sizes
• Smooth navigation between screens


Data Persistence
• All menu data stored locally using AsyncStorage
• Data persists across app sessions
• Default menu items provided for first-time users


Screen Flow
1. **Login Screen** - Chef authentication or customer access
2. **Menu List** - Browse all menu items with filtering
3. **Menu Detail** - View detailed information about items
4. **Chef Dashboard** - (Authenticated chefs only) Manage menu
5. **Edit Menu Item** - Add or edit menu items


Customization

Adding New Categories

Edit the `categories` array in the relevant screen files to add new food categories.


Styling

The app uses a consistent color scheme:
• Primary: `#FF6B35` (Orange)
• Success: `#4CAF50` (Green)
• Error: `#F44336` (Red)
• Info: `#2196F3` (Blue)


Data Storage

Currently uses AsyncStorage for local storage. Can be extended to use:
• Firebase Firestore
• REST API
• GraphQL
• Other backend services


Future Enhancements
• Online ordering system
• Customer reviews and ratings
• Multi-chef support
• Real-time menu updates
• Push notifications for special offers
• Payment integration
• Table reservation system


Troubleshooting

Common Issues
1. **Metro bundler issues**
- Clear cache: `expo start -c`

2. **Navigation issues**
- Ensure all dependencies are installed
- Check screen name consistency in navigation

3. **AsyncStorage issues**
- Clear app data on device
- Check async storage permissions


Support

For issues or questions, refer to:
• Expo documentation: https://docs.expo.dev/
• React Native documentation: https://reactnative.dev/
• React Navigation: https://reactnavigation.org/


⸻


Built with \u2764\ufe0f using React Native and Expo
