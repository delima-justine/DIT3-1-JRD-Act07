# DIT3-1-JRD-Act07

1. What did you learn about using fragments and navigation components?
  - I learned that fragments are reusable UI modules that allow for flexible and adaptive layouts. The Navigation Component simplifies fragment navigation by providing a centralized navigation graph. This graph visually represents the app's flow and handles fragment transactions and the back stack automatically. This approach promotes a modern, single-activity architecture. It makes managing complex UI flows much cleaner and less error-prone.

2. How did you make your UI adaptive to screen size or orientation?
  - To make the UI adaptive, you would create alternative layout resource folders like `layout-land` or `layout-sw600dp`. In these folders, you can provide different layout files for the same screen. For example, a `BottomNavigationView` that is suitable for portrait mode can be replaced with a `NavigationRailView` in landscape mode. This allows the app to optimize its user interface for different screen sizes and orientations. While not yet implemented, this is the standard approach to address the layout validation warnings.

3. What challenges did you face when combining Bottom Navigation and
  Tabs?
  - A key challenge was a runtime crash caused by a subtle timing issue when initializing the NavController. This was resolved by using a more robust method to get the NavController from the NavHostFragment. Another challenge was ensuring the correct Material Components theme was applied, as its absence caused the layout preview to fail and the app to crash. Finally, managing nested navigation between the main bottom bar and the inner tab layout requires careful state management. 
