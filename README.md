# 📱 Contacts App Manager (Map-Based)

A modern, interactive contact management application built with vanilla JavaScript using the **Map data structure**. This project demonstrates practical implementation of JavaScript's Map API with full CRUD operations, real-time search, and a beautiful Bootstrap UI.

## ✨ Features

- **Map-Based Storage**: Utilizes JavaScript's native `Map` data structure for efficient key-value pair storage
- **Full CRUD Operations**: Create, Read, Update, and Delete contacts with ease
- **Real-Time Search**: Instant search functionality across contact names and phone numbers
- **Contact Statistics**: View total contacts, recent additions, and last update time
- **Export to JSON**: Download your contacts as a structured JSON file
- **Responsive Design**: Mobile-friendly interface built with Bootstrap 5
- **Interactive UI**: Smooth animations, hover effects, and visual feedback
- **Data Timestamps**: Track when contacts were added and last updated
- **Quick Add Feature**: Pre-filled buttons for quick demo/testing
- **Clear All**: Bulk delete functionality with confirmation


## 📸 Screenshots

### Main Interface
- Clean, organized contact list with hover effects
- Add contact form with input validation
- Real-time statistics dashboard

### Key Features
- Edit contacts inline with smooth transitions
- Search with highlighted results
- Export contacts to JSON format

## 📋 Map Operations Demonstrated

This project showcases the following JavaScript Map methods:

| Method | Usage in App |
|--------|--------------|
| `set()` | Adding and updating contacts |
| `get()` | Retrieving contact information |
| `has()` | Checking if contact exists |
| `delete()` | Removing individual contacts |
| `clear()` | Removing all contacts |
| `size` | Counting total contacts |
| `keys()` | Iterating through contact names |
| `values()` | Accessing contact data |
| `entries()` | Getting key-value pairs |

## 🎯 Core Functionality

### Contact Class
```javascript
class Contact {
    constructor(name, phone) {
        this.name = name;
        this.phone = phone;
        this.addedAt = new Date().toLocaleString();
        this.lastUpdated = new Date().toLocaleString();
    }
}
```

### Map Operations
- **Add Contact**: `contactsMap.set(name, contact)`
- **Get Contact**: `contactsMap.get(name)`
- **Check Existence**: `contactsMap.has(name)`
- **Delete Contact**: `contactsMap.delete(name)`
- **Clear All**: `contactsMap.clear()`

## 🎮 How to Use

### Adding a Contact
1. Enter contact name in the "Name" field (this becomes the Map key)
2. Enter phone number in the "Phone" field (this becomes the Map value)
3. Click "Add Contact" or press Enter

### Searching Contacts
1. Type in the search box to filter contacts by name or phone number
2. Results update in real-time
3. Click "Clear Search" to reset

### Editing a Contact
1. Click the "Edit" button on any contact
2. Modify the phone number in the edit form
3. Click "Update Contact" to save changes

### Deleting a Contact
1. Click the "Delete" button on any contact
2. Confirm the deletion in the popup dialog

### Exporting Contacts
1. Click "Export to JSON" button
2. Download file will contain all contacts with metadata
3. File format: `contacts_export_YYYY-MM-DD.json`

## 📄 Project Structure

```
contacts-app-manager/
│
├── index.html          # Main HTML structure
├── script.js           # JavaScript logic (Map implementation)
```

## 🔑 Key Concepts Learned

- **Map vs Object**: Why Map is better for key-value storage
- **CRUD Operations**: Complete implementation of Create, Read, Update, Delete
- **ES6 Classes**: Object-oriented contact management
- **DOM Manipulation**: Dynamic UI updates
- **Event Handling**: User interactions and keyboard shortcuts
- **Data Export**: Converting Map to JSON format
- **Local Search**: Filtering and highlighting results
- **Bootstrap Components**: Cards, forms, badges, alerts

## 🌟 Advanced Features

### Smart Contact Management
- Duplicate prevention using `map.has()`
- Automatic timestamp tracking
- Recent contacts counter (last 24 hours)

### User Experience
- Keyboard shortcuts (Enter to add/navigate)
- Hover effects on contact items
- Toast notifications for all actions
- Smooth scroll to edit form
- Empty state messages

### Data Handling
- JSON export with metadata
- Structured contact objects
- Sorted alphabetical display
- Search result highlighting


## 🔮 Future Enhancements

- [ ] Import contacts from JSON
- [ ] Add categories/tags to contacts
- [ ] Email field support
- [ ] Profile pictures for contacts
- [ ] LocalStorage persistence
- [ ] Print contact list
**Happy Coding!** 🚀

*Built with ❤️ using JavaScript Maps*
