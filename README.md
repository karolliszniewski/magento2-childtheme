
To edit: `vendor/magento/theme-frontend-luma/Magento_Theme/web/css/source/`
```bash
app/design/frontend/AnimeKingdom/AnimeTheme
├── registration.php
├── theme.xml
└── web
    ├── css
    │   └── source
    │       ├── _extend.less
    │       └── pages
    │           └── _homepage.less
    └── images 
```

```
vendor/magento/module-theme
├── Api              - Defines interfaces for core theme functionalities.
├── Block            - Holds backend logic for rendering data in templates.
├── Console          - Contains CLI commands for theme management.
├── Controller       - Manages HTTP requests related to themes.
├── CustomerData     - Handles customer data updates (e.g., mini cart).
├── Helper           - Provides utility functions for repeated tasks.
├── i18n             - Translation files for multilingual support.
├── Model            - Core business logic and settings for themes.
├── Observer         - Listens to Magento events (e.g., theme save).
├── Plugin           - Modifies behavior of other classes (interceptors).
├── Setup            - Installation/upgrade scripts for theme database setup.
├── Test             - Unit and integration tests for theme module.
├── Ui               - UI components (forms, grids) for theme module.
├── ViewModel        - Data providers for UI components.
├── view             - Layout, templates, and static assets (CSS, JS).
├── etc              - Configuration files (module, ACL, etc.).
├── registration.php - Registers the theme module in Magento.
├── composer.json    - Module dependencies and metadata for Composer.
├── LICENSE.txt      - License for the theme module.
└── LICENSE_AFL.txt  - Alternative license for the theme module.
```


Here’s a breakdown of the folders in `app/code/Aware/Crud` and their functions in the Magento 2 Aware Crud module setup:

- **Block**: Contains PHP classes for blocks used in the module. Blocks are backend logic containers that prepare data for rendering in the templates (PHTML files). They help connect Magento’s data with its frontend display.

- **Controller**: Contains classes for handling HTTP requests related to the module. For example, controllers manage page requests, loading the correct templates, and displaying module-related content on the frontend.

- **etc**: Contains configuration files for the module, such as module declaration (`module.xml`), routes (`routes.xml`), and database schema (`db_schema.xml`).

- **registration.php**: Registers the module with Magento, allowing it to be recognized and loaded by the system.

- **view**: Contains the XML layout files, template files, and static resources (e.g., CSS, JavaScript) used for rendering the module in the frontend. It also has the module’s default view-related configuration.

- **Model**: Contains core business logic and data models related to the module, such as data manipulation and retrieval.

- **Helper**: Contains helper classes with utility functions used across the module. Helpers often perform repeated or complex tasks that can be called from multiple places within the module.

- **Test**: Contains unit and integration tests for the module’s functionality, ensuring that changes do not break the expected behavior.

- **Plugin**: Contains plugins (interceptors) that modify or extend the behavior of methods in other classes. Plugins enable customization without directly overriding core files.

- **Setup**: Contains setup scripts that run during module installation or upgrade, usually to set up database tables or configurations required by the module.

- **i18n**: Holds translation files (.csv format) for module-related phrases. These files allow the module to support multiple languages by providing localized text.

- **Observer**: Contains event observers, which listen to Magento events (like `module_save_after`) and execute specific actions in response.

- **Api**: Contains PHP interfaces that define core functionalities related to the module, such as managing data and customizations. These are used by other parts of Magento to interact with the module in a standardized way.

- **Console**: Contains console commands related to the module, which can be executed in the Magento command-line interface (CLI) for management tasks.

