# [Any JSON CMS](http://anyjsoncms.com)

Open source headless CMS that could help manage and deliver any JSON to any app.

### Basic usage

#### Create a model

Model is a schema which gives an answer: how does your content entry should look like?

#### Create an entry

Entry is content itself based on corresponding model.

#### Create an API Key

Any client requesting content from the API needs to provide an API Key.

#### Fetch your entries

Fetch your entries as a JSON and use them in any app.

```sh
curl https://api.anyjsoncms.com/entries -H "ApiKey: f7908f51399671456cd33a69c99ac021a08078c6"
```

You will get:
```sh
[
   {
      "id":"5ce9743a69593f074d954c59",
      "identificator":"Interstellar",
      "value":{
         "info":"Movie info",
         "producer":{
            "name":"Nolan",
            "surname":"Christopher"
         },
         "title":"Interstellar"
      },
      "modelId":"5ce9720069593f074d954c58"
   }
]
```

### Installation

Any JSON CMS consists of two parts. [Admin application server](https://github.com/evmizulin/cms-admin) and [API server](https://github.com/evmizulin/cms-api).
