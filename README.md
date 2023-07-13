# Drupal Configurations

### Contents:

- [Image Styles](https://github.com/davidloop/drupal-configurations/tree/main/Image%20Styles)
- [Responsive Preview Device](https://github.com/davidloop/drupal-configurations/tree/main/Responsive%20Preview%20Device)
- [Site Studio - Custom Styles - Button](https://github.com/davidloop/drupal-configurations/tree/main/Site%20Studio/Custom%20Styles/Button)
- [Site Studio - Custom Styles - Layout](https://github.com/davidloop/drupal-configurations/tree/main/Site%20Studio/Custom%20Styles/Layout)
- [Site Studio - Helpers - Styling](https://github.com/davidloop/drupal-configurations/tree/main/Site%20Studio/Helpers/Styling)
- [Site Studio - Components - Basic Components](https://github.com/davidloop/drupal-configurations/tree/main/Site%20Studio/Components/Basic%20Components)
- [Site Studio - Components - Card Components](https://github.com/davidloop/drupal-configurations/tree/main/Site%20Studio/Components/Card%20Components)

<p>&nbsp;</p>

### Theme:

#### Suggest the content type as a page.html.twig file name
```php
/**
 * Implements theme_suggestions_page_alter() for page.html.twig.
 */
function THEME_theme_suggestions_page_alter(array &$suggestions, array $variables) {
  $node = \Drupal::routeMatch()->getParameter('node');
  if ($node instanceof \Drupal\node\NodeInterface) {
    $suggestions[] = 'page__' . $node->bundle();
  }
}
```
