# cafebazaar_market

flutter plugin for cafebazaar android market (only works on android)

## Getting Started

### Go to Application page on Bazaar

```dart
//launches application page on bazaar app if bazaar is installed
CafebazaarMarket.showProgramPage();
```

### Comment

```dart
//launches comment bazaar dialog
CafebazaarMarket.setComment();
```

### Developer page

```dart
//launches developer page on bazaar
CafebazaarMarket.showDeveloperPage("your_id");
```

### Cafe Bazaar login page

```dart
//launches bazaar login page
CafebazaarMarket.showCafebazzarLogin();
```

### Checking for update (if newer version is available)

```dart
bool isUpdateAvailable = await CafebazaarMarket.isUpdateAvailable();
 if(isUpdateAvailable) {
    CafebazaarMarket.goToAppPageOnBazaar();
    //or just show a dialog ask if user wants to update then call CafebazaarMarket.goToAppPageOnBazaar();
 }
```