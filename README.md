## Laravel Nova Big Filter Package

1. [Installation](#user-content-installation)
2. [Usage](#user-content-usage)

## Installation

You can install the package in to a Laravel app that uses [Nova](https://nova.laravel.com) via composer:

```bash
composer require nrml-co/nova-big-filter
```

## Usage

You need to add card to resource with specified filter.

```php

use NrmlCo\NovaBigFilter\NovaBigFilter;
use App\Nova\Filters\YourFilter;
use App\Nova\Filters\YourOtherFilter;

public function filters()
{
    return [
        new YourFilter,
        new YourOtherFilter,
    ];
}

public function cards()
{
    return [        
        new NovaBigFilter,
    ];
}
```