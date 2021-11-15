# KIP-28: OEC Validator Profile

| Author   | Ocean Fan (@OEC)  |
| -------  | --------------------- |
| Status   | Implemented           |
| Type     | Standard Track        |
| Category | Core                  |
| Created  | 2020-8-4              |

## 1. Summary

This KIP sets up a validator profile template for validators to apply to.

## 2. Abstract

KIP-28 Proposal is about a standard of validator profile. Validators should fill in their profile following the template and put their profile on their websites like http://www.yourwebsites.com/validator.json  

## 3. Status

This KIP is implemented.

## 4. Motivation

This KIP make users know more about OEC Validators Info. When validators finished their profile, it'll be easy for delegators or blockchain explorers to get information of validators. 

## 5. Specification

### Validator Profile Template

``` json
{
  "validator_name": "name of validator account",
  "public_key": "Public key for validator account",
  
  "introduction": {
    "en": "Validator description",
    "zh": ""
  },
 
  "org": {
    "name": "Organization name",
    "website": "",
    "email": "",
    "branding":{
      "logo_256":"http://www.xxxxx.com/logo/OEC-256.png",
      "logo_1024":"http://www.xxxxx.com/logo/OEC-1024.png",
      "logo_svg":"http://www.xxxxx.com/logo/OEC-logo.svg"
      
    },
    "location": "City, Country",
    "social_network": {
      "twitter": "https://twitter.com/your-awesome-project",
      "facebook": "https://www.facebook.com/your-awesome-project",
      "github": "https://github.com/your-awesome-project",
      "telegram": "https://t.me/your-awesome-project",
      "steemit": "https://steemit.com/@your-awesome-project"
    }
  },
   "nodes": [
    {
      "location": {
        "name": "OKExNode1",
        "country": "CN",
        "latitude": 40.060599,
        "longitude": 116.32371
      },
      "p2p_endpoint": "",
      "rpc_endpoint": "",
      "rest_endpoint": ""
    },
    {
      "location": {
        "name": "OKExNode2",
        "country": "CN",
        "latitude": 40.060599,
        "longitude": 116.32371
      },
      "p2p_endpoint": "",
      "rpc_endpoint": "",
      "rest_endpoint": ""
    }
  ]
}
```


## 6. License

The content is licensed under [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

 
