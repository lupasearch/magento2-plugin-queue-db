# LupaSearch Magento 2 Db Queue Compatibility Extension

## About extension

The primary [LupaSearch Magento 2 extension](https://github.com/lupasearch/magento2-plugin) assumes RabbitMQ is available as the default queuing system. When RabbitMQ is not part of your project’s infrastructure, the core plugin may not function correctly due to its reliance on AMQP protocols.

This compatibility extension resolves that issue by enabling LupaSearch extension to work seamlessly with MySQL queues.

## Installation

1. Add extension using Composer:

```
composer require lupasearch/magento2-lupasearch-plugin-queue-db
```

2. Run the necessary setup and compilation commands to enable the extension:

```
bin/magento module:enable LupaSearch_LupaSearchPluginQueueDb
bin/magento setup:upgrade
bin/magento setup:di:compile
```
