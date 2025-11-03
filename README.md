SauceTestAutomation

1. To start the application, run the following command : python main.py
2. Configuration-
   Configuration settings can be modified in the config/config.json file.
   base_url – The URL of the application under test
   username / password – Login credentials
   checkout – User details for checkout user
   Products – List of products to add to cart
   sort_by – Sorting option for inventory page
3.Project Structure:
  Config/ config json- configuration 
  Pages/ Implements the Page Object Model each page of the application is represented as a separate class:
  LoginPage.py – actions for the login screen
  InventoryPage.py – actions for the product listing page
  CartPage.py – actions for the shopping cart
  CheckoutInformationPage.py – filling in user details during checkout
  OrderComplete.py – validations for the order completion page
  UI/ locator- contains locators or selectors (XPath, CSS) for UI elements.
  Utils/ Extract_config.py – loads and extracts values from the JSON configuration.
  core/Base_page.py   functionality shared across the project.a base class with common methods
  (e.g., click_button, verify_page_title, error_mes). ➝ All Page Objects inherit from this.
  logs/ Stores log files generated during test execution.


main.py The main entry point of the project. ➝ Orchestrates the entire test flow: login, adding products, checkout, order completion, and screenshot capture on failure.

