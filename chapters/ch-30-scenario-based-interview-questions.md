# CH-30: Scenario-Based Interview Questions

[← Back to Roadmap](../README.md)

---

<a id="301-how-would-you-add-a-custom-attribute-to-the-product-and-expose-it-via-rest-api"></a>
### 30.1 "How would you add a custom attribute to the product and expose it via REST API?"

- [ ] **30.1** "How would you add a custom attribute to the product and expose it via REST API?"
<a id="302-how-would-you-override-a-core-magento-class"></a>
### 30.2 "How would you override a core Magento class?" — Plugin first, then Preference

- [ ] **30.2** "How would you override a core Magento class?" — Plugin first, then Preference
<a id="303-the-site-is-slow-after-a-deploy"></a>
### 30.3 "The site is slow after a deploy — how do you debug?" — Profiler, logs, cache, indexers

- [ ] **30.3** "The site is slow after a deploy — how do you debug?" — Profiler, logs, cache, indexers
<a id="304-design-an-inventory-sync-system-between-amazon-and-magento"></a>
### 30.4 "Design an inventory sync system between Amazon and Magento" — Queue, MSI, idempotency

- [ ] **30.4** "Design an inventory sync system between Amazon and Magento" — Queue, MSI, idempotency
<a id="305-how-would-you-create-a-custom-payment-gateway"></a>
### 30.5 "How would you create a custom payment gateway?" — Redirect flow, webhook, order sync

- [ ] **30.5** "How would you create a custom payment gateway?" — Redirect flow, webhook, order sync
<a id="306-how-would-you-implement-a-custom-shipping-carrier"></a>
### 30.6 "How would you implement a custom shipping carrier?" — `AbstractCarrier`, `collectRates()`

- [ ] **30.6** "How would you implement a custom shipping carrier?" — `AbstractCarrier`, `collectRates()`
<a id="307-how-would-you-add-a-new-step-to-the-checkout"></a>
### 30.7 "How would you add a new step to the checkout?" — Hyva checkout customization, step component

- [ ] **30.7** "How would you add a new step to the checkout?" — Hyva checkout customization, step component
<a id="308-how-would-you-build-a-semantic-product-search"></a>
### 30.8 "How would you build a semantic product search?" — ES embedding, kNN, RAG pipeline

- [ ] **30.8** "How would you build a semantic product search?" — ES embedding, kNN, RAG pipeline
<a id="309-how-do-you-prevent-a-plugin-from-running-in-a-specific-area"></a>
### 30.9 "How do you prevent a plugin from running in a specific area?" — Area check in plugin logic

- [ ] **30.9** "How do you prevent a plugin from running in a specific area?" — Area check in plugin logic
<a id="3010-how-would-you-debug-a-cron-job-that-is-not-running"></a>
### 30.10 "How would you debug a cron job that is not running?" — `cron_schedule` table, group config, log check

- [ ] **30.10** "How would you debug a cron job that is not running?" — `cron_schedule` table, group config, log check

---

## 🔖 Quick Reference — Key Files & Commands

### Essential CLI Commands
```bash
bin/magento setup:upgrade
bin/magento setup:di:compile
bin/magento setup:static-content:deploy -f
bin/magento cache:clean
bin/magento cache:flush
bin/magento indexer:reindex
bin/magento module:enable Vendor_Module
bin/magento queue:consumers:start consumerName
```

### Key Config Files Per Topic
| Topic | File |
|-------|------|
| DI / Plugins | `etc/di.xml` |
| Routes (frontend) | `etc/frontend/routes.xml` |
| Routes (admin) | `etc/adminhtml/routes.xml` |
| Events | `etc/events.xml` (or area-specific) |
| Web API | `etc/webapi.xml` |
| GraphQL | `etc/schema.graphqls` |
| Cron | `etc/crontab.xml` |
| ACL | `etc/acl.xml` |
| System Config | `etc/adminhtml/system.xml` |
| Default Config Values | `etc/config.xml` |
| DB Schema | `etc/db_schema.xml` |
| Message Queue | `etc/queue.xml`, `etc/communication.xml` |
| Extension Attributes | `etc/extension_attributes.xml` |

### Design Patterns — Quick Map
| Pattern | Magento Example |
|---------|----------------|
| Singleton | Shared DI objects |
| Factory | `ProductFactory`, `OrderFactory` |
| Repository | `ProductRepositoryInterface` |
| Service Contract | `Api/ProductRepositoryInterface` |
| Observer | `events.xml` + Observer class |
| Plugin | `di.xml` `<plugin>` + Plugin class |
| Proxy | `SomeClassProxy` in `di.xml` |
| Strategy | Carrier `collectRates()` |
| Composite | Layout block tree |
| Decorator | Plugin chain wrapping |

---
