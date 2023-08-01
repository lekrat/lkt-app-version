# LKT App Version

## Installation

```bash
composer require lkt/app-version
```

## Setup app version

### From composer.json file
```php
\Lkt\AppVersion::readFromComposerFile(__DIR__ . '/path/to/composer.json');
```

### Manual setup
```php
\Lkt\AppVersion::setVersion(1, 0, 0); // Major, Minor, Patch
\Lkt\AppVersion::setVersion('1.0.0'); // All-in-one Major.Minor.Patch
```

## Retrieve version
```php
\Lkt\AppVersion::get(); // Returns version as a dot separated string
\Lkt\AppVersion::getAsNumber(); // Returns version as a number
```