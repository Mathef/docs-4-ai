# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/mockup-generator

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Mockup Generator API

On this page

# Mockup Generator API

You can use this API to generate mockups for your products.

PrintfulStoreClient.mockupGenerator

Printful API Reference

Source

## Create a mockup generation task​

Printful API Reference

Creates an asynchronous mockup generation task. Generation result can be
retrieved using

Method

PrintfulStoreClient.mockupGenerator.createMockupTask(id: number, mockup_task:
MockupTask)

Arguments

id - Product ID.

mockup_task - Mockup Task Info

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Retrieve product variant printfiles​

Printful API Reference

List of printfiles available for products variants. Printfile indicates what
file resolution should be used to create a mockup or submit an order.

Method

PrintfulStoreClient.mockupGenerator.getProductVariantPrintFiles(id: number,
orientation?: Orientation, technique?: string)

Arguments

id - Product ID.

Optional orientation - Enum: \"horizontal\" \"vertical\", Optional orientation
for wall art product printfiles. Allowed values: horizontal, vertical

Optional technique - Optional technique for product. This can be used in cases
where product supports multiple techniques like DTG and embroidery

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Mockup generation task result​

Printful API Reference

Returns asynchronous mockup generation task result. If generation task is
completed, it will contain a list of generated mockups.

Method

PrintfulStoreClient.mockupGenerator.getMockupTaskResult(task_key: string)

Arguments

task_key - Task key retrieved when creating the generation task.

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Layout templates​

Printful API Reference

Retrieve list of templates that can be used for client-side positioning.

Method

PrintfulStoreClient.mockupGenerator.getLayoutTemplates(id: number,
orientation?: Orientation, technique?: string)

Arguments

id - Product ID. Optional orientation - Enum: \"horizontal\" \"vertical\",
Optional orientation for wall art product printfiles. Allowed values:
horizontal, vertical Optional technique - Optional technique for product. This
can be used in cases where product supports multiple techniques like DTG and
embroidery

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Store Information API

Next

Warehouse Products API

  * Create a mockup generation task
  * Retrieve product variant printfiles
  * Mockup generation task result
  * Layout templates

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/contributions/contributing

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

  * Contribution

    * contributing
    * testing

  *   * Contribution
  * contributing

# contributing

Edit this page

Previous

Contribution

Next

testing

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/oauth

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * OAuth API

On this page

# OAuth API

OAuth API allows receiving data for token.

PrintfulStoreClient.oauth

Printful API Reference

Source

## Get scopes for token​

Printful API Reference

Returns a list of scopes associated with the token.

Method

PrintfulStoreClient.oauth.getScopes()

Arguments

None

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    const STORE_TOKEN = \"YOUR STORE TOKEN\";  
      
    const client = createPrintfulStoreClient(STORE_TOKEN);  
      
    // Must call within an async block  
    const {result, error, code} = await client.oauth.getScopes();  
    
```

Edit this page

Previous

Store Level Client

Next

Catalog API

  * Get scopes for token

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/file-library

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * File Library API

On this page

# File Library API

You can use this API to directly add files to the library, and later use File
IDs when creating orders.

PrintfulStoreClient.fileLibrary

Printful API Reference

Source

## Add a new file​

Printful API Reference

Adds a new File to the library by providing URL of the file.

Method

PrintfulStoreClient.fileLibrary.addFile(fileData: File)

Arguments

fileData - Information about file being added

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Get file​

Printful API Reference

Returns information about the given file.

Method

PrintfulStoreClient.fileLibrary.getFile(id: number | string)

Arguments

id - File ID.

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Return available thread colors from provided image URL​

Printful API Reference

Returns colors in hexadecimal format.

Returned thread colors are matched as closely as possible to provided image
colors.

Method

PrintfulStoreClient.fileLibrary.getThreadColors(file_url: string)

Arguments

file_url - URL to file

Example Usage:

```

    
    
    //Soon to be added  
    
```

Edit this page

Previous

Orders API

Next

Shipping Rate API

  * Add a new file
  * Get file
  * Return available thread colors from provided image URL

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/products

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Products API

On this page

# Products API

The Products API resource lets you create, modify and delete products in a
Printful store based on the Manual orders / API platform

PrintfulStoreClient.products

Printful API Reference

Source

## Get Sync Products​

Printful API Reference

Returns a list of Sync Product objects from your custom Printful store.

Method

PrintfulStoreClient.products.getAllSyncProducts(offset?: number, limit?:
number, category_id?: string)

Arguments

Optional offset - Offset for Paging

Optional limit - Limit items for Paging

Optional category_id - A comma-separated list of Category IDs of the Products
that are to be returned

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: products, paging, error} = await client.products.getAllSyncProducts();  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(products);  
      console.log(paging);  
    }  
    
```

## Get a Sync Product​

Printful API Reference

Get information about a single Sync Product and its Sync Variants.

Method

PrintfulStoreClient.products.getSyncProduct(id: number | string)

Argument

id - Sync Product ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: product, error} = await client.products.getSyncProduct(314179759);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(product);  
    }  
    
```

## Create a new Sync Product​

Printful API Reference

Creates a new Sync Product together with its Sync Variants. See Examples

Method

PrintfulStoreClient.products.createSyncProduct(sync_product: SyncProduct,
sync_variants: Array<SyncVariant>)

Arguments

sync_product - Information about the SyncProduct

sync_variants - Information about the Sync Variants

Example Usage

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
    import { SYNC_PRODUCT, SYNC_VARIANTS } from \"./data/products\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: product, error} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(product);  
    }  
    
```

Where ./data/products contains the following data:

```

    
    
    export const SYNC_PRODUCT = {  
      \"name\": \"API product Bella\",  
      \"thumbnail\": \"https://example.com/image.jpg\"  
    }  
      
    export const SYNC_VARIANTS = [  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4011,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      },  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4012,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      }  
    ]  
    
```

## Delete a Sync Product​

Printful API Reference

Deletes a Sync Product with all of its Sync Variants.

Method

PrintfulStoreClient.products.deleteSyncProduct(id: number | string)

Arguments

id - Sync Product ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
    import { SYNC_PRODUCT, SYNC_VARIANTS } from \"./data/products\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: product} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);  
    const {result: deletedProduct, error} = await client.products.deleteSyncProduct(product.id)  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(deletedProduct);  
    }  
    
```

Where ./data/products contains the following data:

```

    
    
    export const SYNC_PRODUCT = {  
      \"name\": \"API product Bella\",  
      \"thumbnail\": \"https://example.com/image.jpg\"  
    }  
      
    export const SYNC_VARIANTS = [  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4011,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      },  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4012,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      }  
    ]  
    
```

## Modify a Sync Product​

Printful API Reference

Modifies an existing Sync Product with its Sync Variants.

Method

PrintfulStoreClient.products.modifySyncProduct(id: number | string, sync_product?: OptionalSyncProduct, sync_variants?: Array<OptionalSyncVariant>)

Arguments

id - Sync Product ID (integer) or External ID (if prefixed with @)

sync_product - Information about the SyncProduct

sync_variants - Information about the Sync Variants

Example Usage:

```

    
    
    import { createPrintfulStoreClient } from \"printful-sdk-js\";  
    import { SYNC_PRODUCT, SYNC_PRODUCT_2, SYNC_VARIANTS, MODIFIED_SYNC_VARIANT } from \"./data/products\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: {id}} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);  
    const {result: product, error} = await client.products.modifySyncProduct(id, SYNC_PRODUCT_2, SYNC_VARIANTS);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(product);  
    }  
    
```

Where ./data/products contains the following data:

```

    
    
    export const SYNC_PRODUCT = {  
      \"name\": \"API product Bella\",  
      \"thumbnail\": \"https://example.com/image.jpg\"  
    }  
      
    export const SYNC_PRODUCT_2 = {  
      \"name\": \"API product Bella Modified\",  
      \"thumbnail\": \"https://example.com/image.jpg\"  
    }  
      
    export const SYNC_VARIANTS = [  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4011,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      },  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4012,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      }  
    ]  
      
    export const MODIFIED_SYNC_VARIANT = {  
      \"retail_price\": \"420.69\",  
      \"variant_id\": 4013,  
      \"files\": [  
        {  
          \"url\": \"https://example.com/image.jpg\"  
        },  
        {  
          \"type\": \"back\",  
          \"url\": \"https://example.com/image.jpg\"  
        }  
      ]  
    }  
    
```

## Get a Sync Variant​

Printful API Reference

Get information about a single Sync Variant.

Method

PrintfulStoreClient.products.getSyncVariant(id: number | string)

Arguments

id - Sync Variant ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    import { createPrintfulStoreClient } from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: products} = await client.products.getAllSyncProducts();  
    const {result: {sync_variants}} = await client.products.getSyncProduct(products[0].id);  
    const {result: variant, error, code} = await client.products.getSyncVariant(sync_variants[0].id);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(variant);  
    }  
    
```

## Delete a Sync Variant​

Printful API Reference

Deletes a single Sync Variant.

Method

PrintfulStoreClient.products.deleteSyncVariant(id: number | string)

Arguments

id - Sync Variant ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    import { createPrintfulStoreClient } from \"printful-sdk-js\";  
    import { SYNC_PRODUCT, SYNC_VARIANTS } from \"./data/products\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: {id}} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);  
    const {result: {sync_variants}} = await client.products.getSyncProduct(id);  
    const {result: variant, error, code} = await client.products.deleteSyncVariant(sync_variants[0].id);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(variant);  
    }  
    
```

Where ./data/products contains the following data:

```

    
    
    export const SYNC_PRODUCT = {  
      \"name\": \"API product Bella\",  
      \"thumbnail\": \"https://example.com/image.jpg\"  
    }  
      
    export const SYNC_VARIANTS = [  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4011,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      },  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4012,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      }  
    ]  
    
```

## Modify a Sync Variant​

Printful API Reference

Modifies an existing Sync Variant.

Method

PrintfulStoreClient.products.modifySyncVariant(id: number | string, sync_variant: OptionalSyncVariant)

Arguments

id - Sync Variant ID (integer) or External ID (if prefixed with @)

sync_variant - Information about the Sync Variant

Example Usage:

```

    
    
    import { createPrintfulStoreClient } from \"printful-sdk-js\";  
    import { SYNC_PRODUCT, SYNC_VARIANTS, MODIFIED_SYNC_VARIANT } from \"./data/products\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: {id}} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);  
    const {result: {sync_variants}} = await client.products.getSyncProduct(id);  
    const {result: variant, error, code} = await client.products.modifySyncVariant(sync_variants[0].id, MODIFIED_SYNC_VARIANT);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(variant);  
    }  
    
```

Where ./data/products contains the following data:

```

    
    
    export const SYNC_PRODUCT = {  
      \"name\": \"API product Bella\",  
      \"thumbnail\": \"https://example.com/image.jpg\"  
    }  
      
    export const SYNC_VARIANTS = [  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4011,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      },  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4012,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      }  
    ]  
      
    export const MODIFIED_SYNC_VARIANT = {  
      \"retail_price\": \"420.69\",  
      \"variant_id\": 4013,  
      \"files\": [  
        {  
          \"url\": \"https://example.com/image.jpg\"  
        },  
        {  
          \"type\": \"back\",  
          \"url\": \"https://example.com/image.jpg\"  
        }  
      ]  
    }  
    
```

## Create a new Sync Variant​

Printful API Reference

Creates a new Sync Variant for an existing Sync Product. See Examples

Method

PrintfulStoreClient.products.createSyncVariant(id: number | string, sync_variant: SyncVariant)

Arguments

id - Sync Product ID (integer) or External ID (if prefixed with @)

sync_variant - Information about the Sync Variant

Example Usage:

```

    
    
    import { createPrintfulStoreClient } from \"printful-sdk-js\";  
    import { SYNC_PRODUCT, SYNC_VARIANTS, NEW_SYNC_VARIANT } from \"./data/products\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: product} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);  
    const {result: variant, error, code} = await client.products.createSyncVariant(product.id, NEW_SYNC_VARIANT);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(variant);  
    }  
    
```

Where ./data/products contains the following data:

```

    
    
    export const SYNC_PRODUCT = {  
      \"name\": \"API product Bella\",  
      \"thumbnail\": \"https://example.com/image.jpg\"  
    }  
      
    export const SYNC_VARIANTS = [  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4011,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      },  
      {  
        \"retail_price\": \"21.00\",  
        \"variant_id\": 4012,  
        \"files\": [  
          {  
            \"url\": \"https://example.com/image.jpg\"  
          },  
          {  
            \"type\": \"back\",  
            \"url\": \"https://example.com/image.jpg\"  
          }  
        ]  
      }  
    ]  
      
    export const NEW_SYNC_VARIANT = {  
      \"retail_price\": \"420.69\",  
      \"variant_id\": 4013,  
      \"files\": [  
        {  
          \"url\": \"https://example.com/image.jpg\"  
        },  
        {  
          \"type\": \"back\",  
          \"url\": \"https://example.com/image.jpg\"  
        }  
      ]  
    }  
    
```

Edit this page

Previous

Catalog API

Next

Orders API

  * Get Sync Products
  * Get a Sync Product
  * Create a new Sync Product
  * Delete a Sync Product
  * Modify a Sync Product
  * Get a Sync Variant
  * Delete a Sync Variant
  * Modify a Sync Variant
  * Create a new Sync Variant

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/intro

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

  * Contribution

  *   * Intro

On this page

# Intro

## Getting Started​

Get started by installing the package.

### What you\'ll need​

  * Node.js version 16.16 or above:
    * When installing Node.js, you are recommended to check all checkboxes related to dependencies.

## Installing the package​

Install the package by running the following command:

```

    
    
    npm i printful-sdk-js  
    
```

You can type this command into Command Prompt, Powershell, Terminal, or any
other integrated terminal of your code editor.

The command also installs all necessary dependencies you need to run printful-
sdk-js.

## Example Usage​

Basic Example in Code:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    const STORE_TOKEN = \"YOUR STORE TOKEN\";  
      
    const client = createPrintfulStoreClient(STORE_TOKEN);  
      
    // Must call within an async block  
    const {result: products, error} = await client.catalog.getAllProducts();  
      
    if (error){  
      console.error(error);  
    }  
    else{  
      console.table(products);  
    }  
    
```

### Getting an access token​

Read the following guide on Prinful API Docs on Authentication.

> IMPORTANT NOTE: It is advised to keep your API keys safe by storing them in
> a .env file and importing it into your project using a tool like dotenv or
> any equivalent you may have available in your project.

Edit this page

Next

Creating a client

  * Getting Started
    * What you\'ll need
  * Installing the package
  * Example Usage
    * Getting an access token

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/warehouse-products

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Warehouse Products API

On this page

# Warehouse Products API

Warehouse Products API

PrintfulStoreClient.warehouseProducts

Printful API Reference

Source

## Get a list of your warehouse products​

Printful API Reference

Returns a list of warehouse products from your store

Method

PrintfulStoreClient.warehouseProducts.getAllWarehouseProducts(query?: string,
offset?: number, limit?: number)

Arguments

Optional query - Filter by partial or full product name

Optional offset - Number of items per page (max 100)

Optional limit - Result set offset

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Get warehouse product data​

Printful API Reference

Returns warehouse product data by ID

Method

PrintfulStoreClient.warehouseProducts.getWarehouseProduct(id: number | string)

Arguments

id - Product ID

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Mockup Generator API

Next

Approval Sheets API

  * Get a list of your warehouse products
  * Get warehouse product data

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/creating-client

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

  * Contribution

  *   * Creating a client

On this page

# Creating a client

Printful offers 2 levels of access for a client, a Store client and an Account
client.

Currently the SDK only offers support for **Store Clients**. Support for
**Account Clients** is WIP🚧.

## Store Level Client​

To instantiate a client, do the following:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    const STORE_TOKEN = \"YOUR STORE TOKEN\";  
      
    const client = createPrintfulStoreClient(STORE_TOKEN);  
    
```

### Getting an access token​

Read the following guide on Prinful API Docs on Authentication.

> IMPORTANT NOTE: It is advised to keep your API keys safe by storing them in
> a .env file and importing it into your project using a tool like dotenv or
> any equivalent you may have available in your project.

### Submodules of Store Client​

After instantiation, client offers a multitude of submodules that correspond
to the sub-APIs as described by the Printful API Documentation.

Below is a table mapping the SDK submodules to their respective sub-APIs.

> NOTE: Parts of the HTTP responses are abstracted away by the SDK. If you
> would like to investigate further, you are welcome to dive into the source
> code.

SDK Submodule| Printful Sub-API  
---|---  
client.oauth| OAuth API  
client.catalog| Catalog API  
client.products| Products API  
client.orders| Orders API  
client.fileLibrary| File Library API  
client.shippingRate| Shipping Rate API  
client.ecommerceSync| Ecommerce Platform Sync API  
client.countryCodes| Country/State Code API  
client.taxRate| Tax Rate API  
client.webhook| Webhook API  
client.storeInformation| Store Information API  
client.mockupGenerator| Mockup Generator API  
client.warehouseProducts| Warehouse Products API  
client.reports| Reports API  
client.approvalSheets| Approval Sheets API  
  
## Account Level Client​

Support for **Account Clients** is WIP🚧.

Edit this page

Previous

Intro

Next

Store Level Client

  * Store Level Client
    * Getting an access token
    * Submodules of Store Client
  * Account Level Client

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/country-codes

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Country/State Code API

On this page

# Country/State Code API

All state/country codes that Printful accepts can be listed by this API.

PrintfulStoreClient.countryCodes

Printful API Reference

Source

## Retrieve country list​

Printful API Reference

Returns list of countries and states that are accepted by the Printful.

Method

PrintfulStoreClient.countryCodes.getCountryList()

Arguments

None

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Ecommerce Platform Sync API

Next

Tax Rate API

  * Retrieve country list

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/shipping-rate

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Shipping Rate API

On this page

# Shipping Rate API

The Shipping rate API calculates the shipping rates for an order based on the
recipient\'s location and the contents of the order.

PrintfulStoreClient.shippingRate

Printful API Reference

Source

## Calculate shipping rates​

Printful API Reference

Returns available shipping options and rates for the given list of products.

Method

PrintfulStoreClient.shippingRate.calculateShipping(shipping_info:
ShippingInfo)

Arguments

shipping_info - Recipient location information

Example Usage

```

    
    
    //Soon to be added  
    
```

Edit this page

Previous

File Library API

Next

Ecommerce Platform Sync API

  * Calculate shipping rates

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/catalog

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Catalog API

On this page

# Catalog API

Catalog API allows receiving data for a substantial catalog of blank Products
and Variants.

PrintfulStoreClient.catalog

Printful API Reference

Source

## Get Products​

Printful API Reference

Returns list of blank Products available in the Printful Catalog.

Method

PrintfulStoreClient.catalog.getAllProducts(category_id?: string)

Arguments

category_id - A comma-separated list of Category IDs of the Products that are
to be returned

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: products, error} = await client.catalog.getAllProducts();  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.table(products);  
    }  
    
```

## Get Variant​

Printful API Reference

Returns information about a specific Variant and its Product.

Method

PrintfulStoreClient.catalog.getVariant(id: number)

Arguments

id - Product ID.

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: variant, error} = await client.catalog.getVariant(4018);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(variant);  
    }  
    
```

## Get Product​

Printful API Reference

Returns information about a specific product and a list of variants for this
product.

Method

PrintfulStoreClient.catalog.getProduct(id: number)

Arguments

id - Product ID.

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: product, error} = await client.catalog.getProduct(71);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(product);  
    }  
    
```

## Get Product Size Guide​

Printful API Reference

Returns information about the size guide for a specific product.

Method

PrintfulStoreClient.catalog.getSize()

Arguments

id - Product ID.

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: sizeGuide, error} = await client.catalog.getSize(71);  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(sizeGuide);  
    }  
    
```

## Get Categories​

Printful API Reference

Returns list of Catalog Categories available in the Printful.

Method

PrintfulStoreClient.catalog.getAllCategories()

Arguments

None

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: categories, error} = await client.catalog.getCategories();  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(categories);  
    }  
    
```

## Get Category​

Printful API Reference

Returns information about a specific category.

Method

PrintfulStoreClient.catalog.getCategory(id: number)

Arguments

id - Category ID

Example Usage:

```

    
    
    import {createPrintfulStoreClient} from \"printful-sdk-js\";  
      
    // ASYNC BLOCK  
    const client = createPrintfulStoreClient(\"STORE_TOKEN\");  
    const {result: category, error} = await client.catalog.getCategory();  
    // ASYNC BLOCK  
      
    if(error){  
      console.error(error);  
    }else{  
      console.log(category);  
    }  
    
```

Edit this page

Previous

OAuth API

Next

Products API

  * Get Products
  * Get Variant
  * Get Product
  * Get Product Size Guide
  * Get Categories
  * Get Category

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/tax-rate

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Tax Rate API

On this page

# Tax Rate API

You can use this API to gather information about tax rates.

PrintfulStoreClient.taxRate

Printful API Reference

Source

## Get a list of countries for tax calculation​

Printful API Reference

Retrieve state list that requires sales tax calculation

Method

PrintfulStoreClient.taxRate.getCountryTaxList()

Arguments

None

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Calculate tax rate​

Printful API Reference

Calculates sales tax rate for given address if required

Method

PrintfulStoreClient.taxRate.calcTax(recipient: Recipient) _Deprecated_

Arguments

recipient - Recipient address information

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Country/State Code API

Next

Webhook API

  * Get a list of countries for tax calculation
  * Calculate tax rate

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/reports

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Reports API

On this page

# Reports API

The Reports API lets you retrieve reports like the statistics related to the
orders fulfilled for your stores.

PrintfulStoreClient.reports

Printful API Reference

Source

## Get statistics​

Printful API Reference

Returns statistics for specified report types.

Method

PrintfulStoreClient.reports.getStats(date_from: RawDateString , date_to:
RawDateString, report_types: string, currency?: string)

Arguments

date_from - The beginning of the period to get the statistics from (date in
YYYY-MM-DD format). Example: 2022-08-01

date_to - The end of the period to get the statistics from (date in YYYY-MM-DD
format). Example: 2022-08-31

currency - The currency (3-letter code) to return the statistics in. You can
also specify display_currency as the value to get the statistics in the
account\'s display currency. The store currency will be used by default.
Example \"USD\"

report_types - A comma-separated list of report types to be retrieved. Example
\"sales_and_costs,profit\"

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Approval Sheets API

Next

Contribution

  * Get statistics

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/category/store-level-client

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client

# Store Level Client

Submodules available for the Store Level Client.

## 📄️ OAuth API

OAuth API allows receiving data for token.

## 📄️ Catalog API

Catalog API allows receiving data for a substantial catalog of blank Products
and Variants.

## 📄️ Products API

The Products API resource lets you create, modify and delete products in a
Printful store based on the Manual orders / API platform

## 📄️ Orders API

The Orders API allows you to create new orders and confirm them for
fulfillment.

## 📄️ File Library API

You can use this API to directly add files to the library, and later use File
IDs when creating orders.

## 📄️ Shipping Rate API

The Shipping rate API calculates the shipping rates for an order based on the
recipient\'s location and the contents of the order.

## 📄️ Ecommerce Platform Sync API

The ecommerce platform sync API allows you to automatically assign Printful
products and print files to the products in your online store (Shopify,
Woocommerce, etc.) that is linked to Printful.

## 📄️ Country/State Code API

All state/country codes that Printful accepts can be listed by this API.

## 📄️ Tax Rate API

You can use this API to gather information about tax rates.

## 📄️ Webhook API

Webhooks are an API feature that allows your system to receive notifications
about certain events. To set up webhooks, use API requests described below.

## 📄️ Store Information API

You can use this API to gather information about your stores.

## 📄️ Mockup Generator API

You can use this API to generate mockups for your products.

## 📄️ Warehouse Products API

Warehouse Products API

## 📄️ Approval Sheets API

Approval Sheets API

## 📄️ Reports API

The Reports API lets you retrieve reports like the statistics related to the
orders fulfilled for your stores.

Previous

Creating a client

Next

OAuth API

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/webhook

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Webhook API

On this page

# Webhook API

Webhooks are an API feature that allows your system to receive notifications
about certain events. To set up webhooks, use API requests described below.

PrintfulStoreClient.webhook

Printful API Reference

Source

## Get webhook configuration​

Printful API Reference

Returns configured webhook URL and list of webhook event types enabled for the
store

Method

PrintfulStoreClient.webhook.getWebhookConfig()

Arguments

None

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Set up webhook configuration​

Printful API Reference

Use this endpoint to enable a webhook URL for a store and select webhook event
types that will be sent to this URL.

Method

PrintfulStoreClient.webhook.setWebhookConfig(newConfig: WebhookConfig)

Arguments

newConfig - Webhook Configuration

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Disable webhook support​

Printful API Reference

Removes the webhook URL and all event types from the store.

Method

PrintfulStoreClient.webhook.disableWebhookSupport()

Arguments

None

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Tax Rate API

Next

Store Information API

  * Get webhook configuration
  * Set up webhook configuration
  * Disable webhook support

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/ecommerce-sync

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Ecommerce Platform Sync API

On this page

# Ecommerce Platform Sync API

The ecommerce platform sync API allows you to automatically assign Printful
products and print files to the products in your online store (Shopify,
Woocommerce, etc.) that is linked to Printful.

PrintfulStoreClient.ecommerceSync

Printful API Reference

Source

## Get list of Sync Products​

Printful API Reference

Returns list of Sync Product objects from your store.

Method

PrintfulStoreClient.ecommerceSync.getAllEcommProducts(offset?: number, limit?:
number, status?: Status, search?: string)

Arguments

Optional offset - Result set offset

Optional limit - Number of items per page (max 100)

Optional status - Filter by item status (synced/unsynced/all). If only some of
the variants are synced,the product is returned by both unsynced and synced
filters

Optional search - Product search needle

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Get a Sync Product​

Printful API Reference

Get information about a single Sync Product and its Sync Variants

Method

PrintfulStoreClient.ecommerceSync.getEcommProduct(id: number | string)

Arguments

id - Sync Product ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Delete a Sync Product​

Printful API Reference

Deletes a Sync Product with all of its Sync Variants

Method

PrintfulStoreClient.ecommerceSync.deleteEcommProduct(id: number | string)

Arguments

id - Sync Product ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Get a Sync Variant​

Printful API Reference

Get information about a single Sync Variant

Method

PrintfulStoreClient.ecommerceSync.getEcommVariant(id: number | string)

Arguments

id - Sync Variant ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Modify a Sync Variant​

Printful API Reference

Modifies an existing Sync Variant.

Method

PrintfulStoreClient.ecommerceSync.modifyEcommVariant(id: number | string, sync_variant_info: OptionalSyncVariant)

Arguments

id - Sync Variant ID (integer) or External ID (if prefixed with @)

sync_variant_info - Information about the Sync Variant

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Delete a Sync Variant​

Printful API Reference

Deletes configuraton information (variant_id, print files and options) and
disables automatic order importing for this Sync Variant.

Method

PrintfulStoreClient.ecommerceSync.deleteEcommVariant(id: number | string)

Arguments

id - Sync Variant ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Shipping Rate API

Next

Country/State Code API

  * Get list of Sync Products
  * Get a Sync Product
  * Delete a Sync Product
  * Get a Sync Variant
  * Modify a Sync Variant
  * Delete a Sync Variant

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/category/contribution

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

  * Contribution

    * contributing
    * testing

  *   * Contribution

# Contribution

Resources about Contributions

## 📄️ contributing

## 📄️ testing

Previous

Reports API

Next

contributing

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/store-information

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Store Information API

On this page

# Store Information API

You can use this API to gather information about your stores.

PrintfulStoreClient.storeInformation

Printful API Reference

Source

## Change packing slip​

Printful API Reference

Modifies packing slip information of the currently authorized Printful store.

Method

PrintfulStoreClient.storeInformation.changePackingSlip(new_packing_slip:
PackingSlip)

Arguments

new_packing_slip - Packing slip information

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Get basic information about stores​

Printful API Reference

Get basic information about stores depending on the token access level

Method

PrintfulStoreClient.storeInformation.getAllStoresInfo(offset?: number, limit?:
number)

Arguments

Optional offset - Offset for query Optional limit - Limit for query

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Get basic information about a store​

Printful API Reference

Get basic information about a store based on provided ID

Method

PrintfulStoreClient.storeInformation.getStoreInfo(id: number)

Arguments

id - Store ID

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Webhook API

Next

Mockup Generator API

  * Change packing slip
  * Get basic information about stores
  * Get basic information about a store

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/contributions/testing

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

  * Contribution

    * contributing
    * testing

  *   * Contribution
  * testing

# testing

Edit this page

Previous

contributing

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/orders

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Orders API

On this page

# Orders API

The Orders API allows you to create new orders and confirm them for
fulfillment.

PrintfulStoreClient.orders

Printful API Reference

Source

## Get list of orders​

Printful API Reference

Returns list of order objects from your store

Method

PrintfulStoreClient.orders.getAllOrders(offset?: number, limit?: number,
status?: OrderStatus)

Arguments

Optional status - Filter by order status

Optional offset - Result set offset

Optional limit - Number of items per page (max 100)

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Create a new order​

Printful API Reference

Creates a new order and optionally submits it for fulfillment

Method

PrintfulStoreClient.orders.createOrder(newOrder: Order, confirm?: boolean,
update_existing?: boolean)

Arguments

newOrder - information about new order

Optional confirm - Automatically submit the newly created order for
fulfillment (skip the Draft phase)

Optional update_existing - Try to update existing order if an order with the
specified external_id already exists

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Get order data​

Printful API Reference

Returns order data by ID or External ID.

Method

PrintfulStoreClient.orders.getOrder(id: number | string)

Arguments

id - Order ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Cancel an order​

Printful API Reference

Cancels pending order or draft. Charged amount is returned to the store
owner\'s credit card.

Method

PrintfulStoreClient.orders.cancelOrder(id: number | string)

Arguments

id - Order ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Update order data​

Printful API Reference

Updates unsubmitted order and optionally submits it for the fulfillment.

Method

PrintfulStoreClient.orders.updateOrder(id: number | string, orderData: Order, confirm?: boolean)

Arguments

id - Order ID (integer) or External ID (if prefixed with @) orderData - Update
information about the order Optional confirm - Automatically submit the newly
created order for fulfillment (skip the Draft phase)

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Confirm draft for fulfillment​

Printful API Reference

Approves for fulfillment an order that was saved as a draft. Store owner\'s
credit card is charged when the order is submitted for fulfillment.

Method

PrintfulStoreClient.orders.confirmOrder(id: number | string)

Arguments

id - Order ID (integer) or External ID (if prefixed with @)

Example Usage:

```

    
    
    //Soon to be added  
    
```

## Estimate order costs​

Printful API Reference

Calculates the estimated order costs including item costs, print costs (back
prints, inside labels etc.), shipping and taxes

Method

PrintfulStoreClient.orders.estimateOrderCost(orderData: Order)

Arguments

orderData - Information on order for which estimate will be returned

Example Usage:

```

    
    
    //Soon to be added  
    
```

Edit this page

Previous

Products API

Next

File Library API

  * Get list of orders
  * Create a new order
  * Get order data
  * Cancel an order
  * Update order data
  * Confirm draft for fulfillment
  * Estimate order costs

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.




# Scraped content from https://printful-sdk-js.netlify.app/docs/store-level-client/approval-sheets

Skip to main content

Printful SDK JSDocs

GitHubNPM

  * Intro
  * Creating a client
  * Store Level Client

    * OAuth API
    * Catalog API
    * Products API
    * Orders API
    * File Library API
    * Shipping Rate API
    * Ecommerce Platform Sync API
    * Country/State Code API
    * Tax Rate API
    * Webhook API
    * Store Information API
    * Mockup Generator API
    * Warehouse Products API
    * Approval Sheets API
    * Reports API
  * Contribution

  *   * Store Level Client
  * Approval Sheets API

On this page

# Approval Sheets API

Approval Sheets API

PrintfulStoreClient.approvalSheets

Printful API Reference

Source

## Retrieve a list of approval sheets​

Printful API Reference

Retrieve a list of approval sheets confirming suggested changes to files of on
hold orders.

Method

PrintfulStoreClient.approvalSheets.getApprovalSheets()

Arguments

None

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Approve a design​

Printful API Reference

Uses the confirm hash of an approval sheet to approve a design and remove the
hold on an order

Methods

PrintfulStoreClient.approvalSheets.approveDesign(confirm_hash: string, status:
string)

Arguments

confirm_hash - The confirm hash for the approval sheet you would like to
approve.

status - Status value

Example Usage:

```

    
    
    // Soon to be added  
    
```

## Submit changes to an approval sheet​

Printful API Reference

Use this to submit alternative changes to a design that has an approval sheet

Methods

PrintfulStoreClient.approvalSheets.changeApprovalSheet(confirm_hash: string,
changes: ApprovalSheetChanges)

Arguments

confirm_hash - The confirm hash for the approval sheet you would like to
approve.

changes - Data to be submitted to Printful designers

Example Usage:

```

    
    
    // Soon to be added  
    
```

Edit this page

Previous

Warehouse Products API

Next

Reports API

  * Retrieve a list of approval sheets
  * Approve a design
  * Submit changes to an approval sheet

Docs

  * Getting Started

More

  * GitHub
  * NPM

Printful SDK JS Docs. Built with Docusaurus.


