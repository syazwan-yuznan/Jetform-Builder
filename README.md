# WordPress Post Delete Confirmation

A WordPress plugin that adds a stylish confirmation dialog when deleting posts. This plugin is especially useful for frontend post deletion, providing users with a clear confirmation step before permanently removing content.

## Features

- Beautiful, modern confirmation dialog
- Animated overlay with blur effect
- 5-minute time limit for post deletion
- AJAX-based deletion with security checks
- Mobile-responsive design
- Shortcode support for deletion links
- Permission checking to ensure secure deletion

## Installation

1. Download the plugin files
2. Upload them to your `/wp-content/plugins/` directory
3. Activate the plugin through the 'Plugins' menu in WordPress

## Usage

### Basic Usage

The plugin automatically adds the confirmation dialog to your footer and handles post deletion requests.

### Shortcode

Use the `[trash_post_link]` shortcode to generate a deletion link for the current post. The link will only be active for 5 minutes after post creation.

Example:
```php
[trash_post_link]
```

### Integration with JetEngine

The plugin is designed to work with JetEngine dynamic links. Add a dynamic link with the following settings:

1. Set the link source to "Shortcode"
2. Use the shortcode: `[trash_post_link]`
3. Style your link as needed

## Security Features

- Nonce verification for all deletion requests
- Permission checking using WordPress capabilities
- XSS prevention
- AJAX request validation

## Requirements

- WordPress 5.0 or higher
- jQuery (included with WordPress)
- JetEngine plugin (optional, for dynamic listings)

## Customization

### Styling

The plugin includes default styles for the confirmation dialog. You can customize the appearance by adding custom CSS to your theme.

### Time Limit

By default, posts can only be deleted within 5 minutes of creation. To modify this limit, edit the `trash_post_link_shortcode` function.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Support

For support, please open an issue in the GitHub repository.
