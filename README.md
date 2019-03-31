# Introduction

Drupal modules for [AI-based customer insights (AICI)](https://codoma.tech/aici/).

# Installation

1. Method1: (TODO) Once the project is on Drupal, you can install it in the standard drupal way .

2. Method 2: copy the contents of this repository to your `sites/all/modules`.

# Configuration

## Module: You-May-Also-Like

1. Enable the module `You-May-Also-Like`, this will enable the base module `aici` if it's not enabled.
2. Configure the module at `admin/config/aici-ymal`
     1. The algorithm depends heavily on the categorization of your contents (i.e. terms),
     uncategorized contents cannot be processed
     2. Additionally, you need to tell the module how the various categories are related to each other
     this can be configured in the 'categories Relationships' section of the admin page. The quality
     of this configuration affects the quality of the modules recommendations.
3. The module provide a block of related categories


# FAQ

## How is the data collected?

AICI modules store anonymized (i.e. hashed) access information in your site's database.

## Will the collected data be used or shared to a third-party?

No. The collected data is stored in your site's database and is not shared with any external service.
This can be easily verified by checking the modules sources provided here.

## I don't know how to configure category relationships. Or I need better insights for my site.

Every site has its own characteristic categorization and user behaviors. We developed the open-source
version of AICI for the most common case, to provide reasonable insights to as many websites as possible.
If you need customization to your own site, please [contact us](https://codoma.tech/aici/).
