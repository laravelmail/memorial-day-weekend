# Memorial Day Weekend

Professional Memorial Day Weekend email promoting travel and tourism services with special discounts for the long weekend.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Travel & Tourism
- **Message Type:** Events
- **Tags:** discounts, promotions, memorialdayweekend

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/memorial-day-weekend.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/memorial-day-weekend/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.memorial-day-weekend',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
