### Laravel Developer Test Task (Appfront)

### Changes and Code refactoring

- **Code Refactoring:**
    1. Centralized error handling.
    2. Centralized image upload logic.
    3. Centralized notification dispatch logic.
    4. Refactored and improved validation logic.
    5. Added a default placeholder for missing images.
    6. Simplified product update logic by using $product->update($request->except('image')) to update product fields in the updateProduct method.
    7. Graceful handling of missing products.
    8. Defined validation rules for addProduct and updateProduct.
    9. Refactored web.php for better readability and optimization.
    10. Added middleware to prevent unnecessary login attempts for routes while already logged in.
    11. Introduced layout files by creating a common layout and moved inline CSS from <style> tags into a `custom.css` file.
    12. Added a fallback to the environment variable EXCHANGE_RATE in case the API call fails.
    13. Moved the exchange rate fetching logic into a private method getExchangeRate.
    14. Replaced cURL requests with Laravel's Http facade.


### Suggestions
    1. Use soft delete by adding a is_deleted column in database table
    2. Introduce data table for better representation and managing data
