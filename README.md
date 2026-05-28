# Magento 2 Interview Preparation Roadmap
### Nitish Kumar Upadhyay — 3+ Years Experience | Adobe Certified Developer

---

## 📋 Progress Tracker

| Chapter | Topics | Status |
|---------|--------|--------|
| [CH-01: Architecture & Request Lifecycle](chapters/ch-01-architecture-request-lifecycle.md) | 8 topics | [ ] |
| [CH-02: Dependency Injection & Object Manager](chapters/ch-02-dependency-injection-object-manager.md) | 7 topics | [ ] |
| [CH-03: Module Development](chapters/ch-03-module-development.md) | 10 topics | [ ] |
| [CH-04: Plugin System & Interceptors](chapters/ch-04-plugin-system-interceptors.md) | 6 topics | [ ] |
| [CH-05: Events & Observers](chapters/ch-05-events-observers.md) | 5 topics | [ ] |
| [CH-06: Design Patterns in Magento 2](chapters/ch-06-design-patterns-in-magento-2.md) | 10 topics | [ ] |
| [CH-07: Service Contracts & Repositories](chapters/ch-07-service-contracts-repositories.md) | 7 topics | [ ] |
| [CH-08: Database, ORM & EAV Model](chapters/ch-08-database-orm-eav-model.md) | 9 topics | [ ] |
| [CH-09: Declarative Schema & Data Patches](chapters/ch-09-declarative-schema-data-patches.md) | 6 topics | [ ] |
| [CH-10: Caching System](chapters/ch-10-caching-system.md) | 8 topics | [ ] |
| [CH-11: Indexing System](chapters/ch-11-indexing-system.md) | 7 topics | [ ] |
| [CH-12: REST API & Web API](chapters/ch-12-rest-api-web-api.md) | 8 topics | [ ] |
| [CH-13: GraphQL API](chapters/ch-13-graphql-api.md) | 7 topics | [ ] |
| [CH-14: Message Queues & Async Processing](chapters/ch-14-message-queues-async-processing.md) | 6 topics | [ ] |
| [CH-15: Payment Gateway Integration](chapters/ch-15-payment-gateway-integration.md) | 7 topics | [ ] |
| [CH-16: Shipping API Integration](chapters/ch-16-shipping-api-integration.md) | 5 topics | [ ] |
| [CH-17: Multi-Source Inventory (MSI)](chapters/ch-17-multi-source-inventory-msi.md) | 6 topics | [ ] |
| [CH-18: Frontend — Layout XML & Blocks](chapters/ch-18-frontend-layout-xml-blocks.md) | 7 topics | [ ] |
| [CH-19: Frontend — Hyva Theme](chapters/ch-19-frontend-hyva-theme.md) | 7 topics | [ ] |
| [CH-20: UI Components (Admin)](chapters/ch-20-ui-components-admin.md) | 5 topics | [ ] |
| [CH-21: Performance Optimization](chapters/ch-21-performance-optimization.md) | 9 topics | [ ] |
| [CH-22: Search — Elasticsearch & OpenSearch](chapters/ch-22-search-elasticsearch-opensearch.md) | 7 topics | [ ] |
| [CH-23: AI & RAG-Based Search (Your Edge)](chapters/ch-23-ai-rag-based-search-your-edge.md) | 7 topics | [ ] |
| [CH-24: Security Best Practices](chapters/ch-24-security-best-practices.md) | 7 topics | [ ] |
| [CH-25: DevOps, CLI & Deployment](chapters/ch-25-devops-cli-deployment.md) | 7 topics | [ ] |
| [CH-26: Composer & Dependency Management](chapters/ch-26-composer-dependency-management.md) | 4 topics | [ ] |
| [CH-27: Magento 2.3 vs 2.4 vs Adobe Commerce](chapters/ch-27-magento-23-vs-24-vs-adobe-commerce.md) | 5 topics | [ ] |
| [CH-28: Compliance & Tax Integrations](chapters/ch-28-compliance-tax-integrations.md) | 5 topics | [ ] |
| [CH-29: PHP & OOP Concepts for Magento](chapters/ch-29-php-oop-concepts-for-magento.md) | 7 topics | [ ] |
| [CH-30: Scenario-Based Interview Questions](chapters/ch-30-scenario-based-interview-questions.md) | 10 topics | [ ] |

---

## 📚 Chapters

- [CH-01: Architecture & Request Lifecycle](chapters/ch-01-architecture-request-lifecycle.md)
  - [1.1 Magento 2 overall architecture overview — areas, layers, components](chapters/ch-01-architecture-request-lifecycle.md#11-magento-2-overall-architecture-overview)
  - [1.2 Application areas — `frontend`, `adminhtml`, `crontab`, `webapi_rest`, `graphql`, `doc`](chapters/ch-01-architecture-request-lifecycle.md#12-application-areas)
  - [1.3 Request lifecycle — `index.php` → Bootstrap → App → FrontController → Router → Controller](chapters/ch-01-architecture-request-lifecycle.md#13-request-lifecycle)
  - [1.4 Router types — standard, admin, CMS, default (404)](chapters/ch-01-architecture-request-lifecycle.md#14-router-types)
  - [1.5 Controller anatomy — `execute()`, `ResultFactory`, redirect vs page vs JSON response](chapters/ch-01-architecture-request-lifecycle.md#15-controller-anatomy)
  - [1.6 Action URL structure — `frontName/controller/action`](chapters/ch-01-architecture-request-lifecycle.md#16-action-url-structure)
  - [1.7 Magento directory structure — `app/`, `vendor/`, `pub/`, `var/`, `generated/`](chapters/ch-01-architecture-request-lifecycle.md#17-magento-directory-structure)
  - [1.8 Module file structure — `registration.php`, `module.xml`, `etc/`, `Block/`, `Controller/`, `Model/`, `view/`](chapters/ch-01-architecture-request-lifecycle.md#18-module-file-structure)

- [CH-02: Dependency Injection & Object Manager](chapters/ch-02-dependency-injection-object-manager.md)
  - [2.1 What is Dependency Injection — constructor vs method vs property injection](chapters/ch-02-dependency-injection-object-manager.md#21-what-is-dependency-injection)
  - [2.2 `di.xml` configuration — `<preference>`, `<type>`, `<arguments>`, `<virtualType>`](chapters/ch-02-dependency-injection-object-manager.md#22-dixml-configuration)
  - [2.3 Object Manager — role, why not to use it directly in production code](chapters/ch-02-dependency-injection-object-manager.md#23-object-manager)
  - [2.4 Shared vs non-shared instances — singletons and factories](chapters/ch-02-dependency-injection-object-manager.md#24-shared-vs-non-shared-instances)
  - [2.5 Factory classes — when and why to use `SomeClassFactory`](chapters/ch-02-dependency-injection-object-manager.md#25-factory-classes)
  - [2.6 Proxy classes — lazy-loading heavy dependencies, `SomeClassProxy`](chapters/ch-02-dependency-injection-object-manager.md#26-proxy-classes)
  - [2.7 Virtual types — reusing class configuration without creating new classes](chapters/ch-02-dependency-injection-object-manager.md#27-virtual-types)

- [CH-03: Module Development](chapters/ch-03-module-development.md)
  - [3.1 Creating a module from scratch — `registration.php`, `module.xml`, `composer.json`](chapters/ch-03-module-development.md#31-creating-a-module-from-scratch)
  - [3.2 Module load order — `<sequence>` in `module.xml`, dependency resolution](chapters/ch-03-module-development.md#32-module-load-order)
  - [3.3 Module enable/disable — `bin/magento module:enable`, `module_setup` table](chapters/ch-03-module-development.md#33-module-enabledisable)
  - [3.4 Creating a custom controller — frontend and admin routing](chapters/ch-03-module-development.md#34-creating-a-custom-controller)
  - [3.5 Creating a custom admin grid with UI component](chapters/ch-03-module-development.md#35-creating-a-custom-admin-grid-with-ui-component)
  - [3.6 Custom system configuration — `system.xml`, `config.xml`, `acl.xml`](chapters/ch-03-module-development.md#36-custom-system-configuration)
  - [3.7 Adding custom attributes to products, customers, orders](chapters/ch-03-module-development.md#37-adding-custom-attributes-to-products-customers-orders)
  - [3.8 Extension attributes — `extension_attributes.xml`, join directives](chapters/ch-03-module-development.md#38-extension-attributes)
  - [3.9 Custom cron job — `crontab.xml`, cron groups, schedule expression](chapters/ch-03-module-development.md#39-custom-cron-job)
  - [3.10 Custom CLI command — `di.xml` registration, `InputInterface`, `OutputInterface`](chapters/ch-03-module-development.md#310-custom-cli-command)

- [CH-04: Plugin System & Interceptors](chapters/ch-04-plugin-system-interceptors.md)
  - [4.1 Plugin types — Before, Around, After — purpose and signature of each](chapters/ch-04-plugin-system-interceptors.md#41-plugin-types)
  - [4.2 Around plugin — `$proceed()` call, skipping original method, wrapping logic](chapters/ch-04-plugin-system-interceptors.md#42-around-plugin)
  - [4.3 Plugin limitations — final classes, static methods, non-public methods, `__construct`](chapters/ch-04-plugin-system-interceptors.md#43-plugin-limitations)
  - [4.4 Plugin sort order — `sortOrder` attribute and conflict resolution](chapters/ch-04-plugin-system-interceptors.md#44-plugin-sort-order)
  - [4.5 Plugin vs Preference vs Observer — when to choose which](chapters/ch-04-plugin-system-interceptors.md#45-plugin-vs-preference-vs-observer)
  - [4.6 Can you plugin a plugin? — generated interceptor class explanation](chapters/ch-04-plugin-system-interceptors.md#46-can-you-plugin-a-plugin)

- [CH-05: Events & Observers](chapters/ch-05-events-observers.md)
  - [5.1 Event-Observer pattern — `events.xml` structure, `instance` and `method`](chapters/ch-05-events-observers.md#51-event-observer-pattern)
  - [5.2 Area-specific vs global event registration](chapters/ch-05-events-observers.md#52-area-specific-vs-global-event-registration)
  - [5.3 Dispatching custom events — `EventManager::dispatch()`, `DataObject`](chapters/ch-05-events-observers.md#53-dispatching-custom-events)
  - [5.4 Key Magento events — `sales_order_place_after`, `customer_register_success`, `catalog_product_save_after`](chapters/ch-05-events-observers.md#54-key-magento-events)
  - [5.5 Observer best practices — keeping observers lightweight, no heavy DB operations](chapters/ch-05-events-observers.md#55-observer-best-practices)

- [CH-06: Design Patterns in Magento 2](chapters/ch-06-design-patterns-in-magento-2.md)
  - [6.1 Singleton pattern — shared object instances in DI container](chapters/ch-06-design-patterns-in-magento-2.md#61-singleton-pattern)
  - [6.2 Factory pattern — object creation via generated factory classes](chapters/ch-06-design-patterns-in-magento-2.md#62-factory-pattern)
  - [6.3 Repository pattern — data access abstraction over ResourceModels](chapters/ch-06-design-patterns-in-magento-2.md#63-repository-pattern)
  - [6.4 Service Contract pattern — interfaces as stable API layer](chapters/ch-06-design-patterns-in-magento-2.md#64-service-contract-pattern)
  - [6.5 Observer / Event pattern — decoupled event-driven communication](chapters/ch-06-design-patterns-in-magento-2.md#65-observer-event-pattern)
  - [6.6 Plugin / Interceptor pattern — method-level AOP without inheritance](chapters/ch-06-design-patterns-in-magento-2.md#66-plugin-interceptor-pattern)
  - [6.7 Proxy pattern — deferred object initialization for performance](chapters/ch-06-design-patterns-in-magento-2.md#67-proxy-pattern)
  - [6.8 Strategy pattern — swappable algorithms (e.g. shipping rate carriers)](chapters/ch-06-design-patterns-in-magento-2.md#68-strategy-pattern)
  - [6.9 Decorator pattern — wrapping objects to add behavior](chapters/ch-06-design-patterns-in-magento-2.md#69-decorator-pattern)
  - [6.10 Composite pattern — tree structures (e.g. category tree, layout blocks)](chapters/ch-06-design-patterns-in-magento-2.md#610-composite-pattern)

- [CH-07: Service Contracts & Repositories](chapters/ch-07-service-contracts-repositories.md)
  - [7.1 What are service contracts — interfaces in `Api/` folder, why they matter](chapters/ch-07-service-contracts-repositories.md#71-what-are-service-contracts)
  - [7.2 Data interfaces (DTOs) — `Api/Data/`, difference from Model objects](chapters/ch-07-service-contracts-repositories.md#72-data-interfaces-dtos)
  - [7.3 Repository interface methods — `getById()`, `save()`, `delete()`, `getList()`](chapters/ch-07-service-contracts-repositories.md#73-repository-interface-methods)
  - [7.4 `SearchCriteriaInterface` — FilterGroup, Filter, SortOrder, page size](chapters/ch-07-service-contracts-repositories.md#74-searchcriteriainterface)
  - [7.5 `SearchResultsInterface` — returning paginated lists from `getList()`](chapters/ch-07-service-contracts-repositories.md#75-searchresultsinterface)
  - [7.6 Never pass Model across service layer — use Data interfaces instead](chapters/ch-07-service-contracts-repositories.md#76-never-pass-model-across-service-layer)
  - [7.7 Custom repository implementation — ResourceModel usage inside repository](chapters/ch-07-service-contracts-repositories.md#77-custom-repository-implementation)

- [CH-08: Database, ORM & EAV Model](chapters/ch-08-database-orm-eav-model.md)
  - [8.1 EAV model — what it is, why Magento uses it for products and customers](chapters/ch-08-database-orm-eav-model.md#81-eav-model)
  - [8.2 EAV tables — `eav_entity_type`, `catalog_product_entity`, `_varchar`, `_int`, `_decimal`, `_datetime`, `_text`](chapters/ch-08-database-orm-eav-model.md#82-eav-tables)
  - [8.3 Flat model vs EAV — performance difference, flat catalog tables](chapters/ch-08-database-orm-eav-model.md#83-flat-model-vs-eav)
  - [8.4 ResourceModel — extending `AbstractDb`, `_init()`, `_construct()`](chapters/ch-08-database-orm-eav-model.md#84-resourcemodel)
  - [8.5 Collection — `addFieldToFilter()`, `addAttributeToFilter()`, `getSelect()`](chapters/ch-08-database-orm-eav-model.md#85-collection)
  - [8.6 Joining tables in a collection — `getSelect()->join()`, `joinLeft()`](chapters/ch-08-database-orm-eav-model.md#86-joining-tables-in-a-collection)
  - [8.7 `load()` on Model vs using Repository — when each is appropriate](chapters/ch-08-database-orm-eav-model.md#87-load-on-model-vs-using-repository)
  - [8.8 Custom attribute backend types — `varchar`, `int`, `decimal`, `text`, `datetime`](chapters/ch-08-database-orm-eav-model.md#88-custom-attribute-backend-types)
  - [8.9 Source models, backend models, frontend models for custom attributes](chapters/ch-08-database-orm-eav-model.md#89-source-models-backend-models-frontend-models-for-custom-attributes)

- [CH-09: Declarative Schema & Data Patches](chapters/ch-09-declarative-schema-data-patches.md)
  - [9.1 Declarative schema — `db_schema.xml` vs old `InstallSchema` / `UpgradeSchema`](chapters/ch-09-declarative-schema-data-patches.md#91-declarative-schema)
  - [9.2 `db_schema_whitelist.json` — why it's generated and what it controls](chapters/ch-09-declarative-schema-data-patches.md#92-db_schema_whitelistjson)
  - [9.3 Data patches — `DataPatchInterface`, `getDependencies()`, `getAliases()`](chapters/ch-09-declarative-schema-data-patches.md#93-data-patches)
  - [9.4 Schema patches — `SchemaPatchInterface` for structural changes](chapters/ch-09-declarative-schema-data-patches.md#94-schema-patches)
  - [9.5 Revertable patches — implementing `revert()` method](chapters/ch-09-declarative-schema-data-patches.md#95-revertable-patches)
  - [9.6 Patch execution tracking — `patch_list` table, preventing re-runs](chapters/ch-09-declarative-schema-data-patches.md#96-patch-execution-tracking)

- [CH-10: Caching System](chapters/ch-10-caching-system.md)
  - [10.1 Magento cache types — `config`, `layout`, `block_html`, `full_page`, `collections`, `eav`, `translate`, `reflection`](chapters/ch-10-caching-system.md#101-magento-cache-types)
  - [10.2 Cache backend — file system vs Redis — configuration in `env.php`](chapters/ch-10-caching-system.md#102-cache-backend)
  - [10.3 Full Page Cache (FPC) — built-in vs Varnish, how it works](chapters/ch-10-caching-system.md#103-full-page-cache-fpc)
  - [10.4 Hole-punching with ESI (Edge Side Includes) — private blocks in cached pages](chapters/ch-10-caching-system.md#104-hole-punching-with-esi-edge-side-includes)
  - [10.5 Cache tags — how Magento tags blocks, `getCacheKeyInfo()`, `getCacheTags()`](chapters/ch-10-caching-system.md#105-cache-tags)
  - [10.6 Selective cache invalidation — `cache:clean` vs `cache:flush`, `clean()` with tags](chapters/ch-10-caching-system.md#106-selective-cache-invalidation)
  - [10.7 Custom cache type — implementing `FrontendInterface`, registering in `di.xml`](chapters/ch-10-caching-system.md#107-custom-cache-type)
  - [10.8 Redis for sessions — `session.save` config, session locking considerations](chapters/ch-10-caching-system.md#108-redis-for-sessions)

- [CH-11: Indexing System](chapters/ch-11-indexing-system.md)
  - [11.1 What indexers do — why Magento needs them (EAV to flat, price calculation, search)](chapters/ch-11-indexing-system.md#111-what-indexers-do)
  - [11.2 Index modes — `realtime` vs `schedule`, when to use each](chapters/ch-11-indexing-system.md#112-index-modes)
  - [11.3 Key indexers — `catalog_product_price`, `catalogsearch_fulltext`, `cataloginventory_stock`, `catalog_category_product`](chapters/ch-11-indexing-system.md#113-key-indexers)
  - [11.4 Mview (materialized view) — how schedule mode tracks incremental changes](chapters/ch-11-indexing-system.md#114-mview-materialized-view)
  - [11.5 Custom indexer — implementing `IndexerInterface`, registering in `indexer.xml`](chapters/ch-11-indexing-system.md#115-custom-indexer)
  - [11.6 `bin/magento indexer:reindex` — full vs partial reindex](chapters/ch-11-indexing-system.md#116-binmagento-indexerreindex)
  - [11.7 Indexer performance — large catalog considerations, partial indexing triggers](chapters/ch-11-indexing-system.md#117-indexer-performance)

- [CH-12: REST API & Web API](chapters/ch-12-rest-api-web-api.md)
  - [12.1 `webapi.xml` — route, HTTP method, service interface method, resource ACL](chapters/ch-12-rest-api-web-api.md#121-webapixml)
  - [12.2 Auth methods — admin token, customer token, OAuth 1.0a, guest](chapters/ch-12-rest-api-web-api.md#122-auth-methods)
  - [12.3 Exposing custom endpoints — service contract → `webapi.xml` → auto-routing](chapters/ch-12-rest-api-web-api.md#123-exposing-custom-endpoints)
  - [12.4 `SearchCriteria` in REST — filter groups, filters, sorting, pagination via URL params](chapters/ch-12-rest-api-web-api.md#124-searchcriteria-in-rest)
  - [12.5 Async REST API — `async/bulk/` prefix, queue-based processing](chapters/ch-12-rest-api-web-api.md#125-async-rest-api)
  - [12.6 Bulk API operations — `V1/bulk` endpoint, status tracking](chapters/ch-12-rest-api-web-api.md#126-bulk-api-operations)
  - [12.7 REST API versioning — `/V1/`, `/V2/` — backward compatibility contract](chapters/ch-12-rest-api-web-api.md#127-rest-api-versioning)
  - [12.8 Amazon-to-Magento inventory sync — SP-API integration, queue pattern, idempotency](chapters/ch-12-rest-api-web-api.md#128-amazon-to-magento-inventory-sync)

- [CH-13: GraphQL API](chapters/ch-13-graphql-api.md)
  - [13.1 `schema.graphqls` — type definitions, queries, mutations, interfaces](chapters/ch-13-graphql-api.md#131-schemagraphqls)
  - [13.2 Resolver classes — implementing `ResolverInterface`, returning array](chapters/ch-13-graphql-api.md#132-resolver-classes)
  - [13.3 Context object — store scope, customer identity, authorization](chapters/ch-13-graphql-api.md#133-context-object)
  - [13.4 Extending existing Magento GraphQL types — `@resolver`, `@doc` directives](chapters/ch-13-graphql-api.md#134-extending-existing-magento-graphql-types)
  - [13.5 Custom query vs custom mutation — when to use each](chapters/ch-13-graphql-api.md#135-custom-query-vs-custom-mutation)
  - [13.6 N+1 problem in GraphQL — batching with `BatchContractInterface`, deferred resolvers](chapters/ch-13-graphql-api.md#136-n1-problem-in-graphql)
  - [13.7 GraphQL caching — cache resolution, `@cache` directive, Varnish + GraphQL](chapters/ch-13-graphql-api.md#137-graphql-caching)

- [CH-14: Message Queues & Async Processing](chapters/ch-14-message-queues-async-processing.md)
  - [14.1 Queue configuration files — `queue.xml`, `communication.xml`, `topology.xml`](chapters/ch-14-message-queues-async-processing.md#141-queue-configuration-files)
  - [14.2 Publisher → Exchange → Queue → Consumer flow](chapters/ch-14-message-queues-async-processing.md#142-publisher-exchange-queue-consumer-flow)
  - [14.3 RabbitMQ vs MySQL queue — when to use each](chapters/ch-14-message-queues-async-processing.md#143-rabbitmq-vs-mysql-queue)
  - [14.4 Consumer management — `bin/magento queue:consumers:start`, supervisor daemon](chapters/ch-14-message-queues-async-processing.md#144-consumer-management)
  - [14.5 Dead letter queues — failed message handling, retry strategies](chapters/ch-14-message-queues-async-processing.md#145-dead-letter-queues)
  - [14.6 When to use message queues vs synchronous processing — trade-off decisions](chapters/ch-14-message-queues-async-processing.md#146-when-to-use-message-queues-vs-synchronous-processing)

- [CH-15: Payment Gateway Integration](chapters/ch-15-payment-gateway-integration.md)
  - [15.1 Payment method interface — `MethodInterface` vs `AbstractMethod` (legacy)](chapters/ch-15-payment-gateway-integration.md#151-payment-method-interface)
  - [15.2 Payment flow — `authorize()`, `capture()`, `void()`, `refund()`, `cancel()`](chapters/ch-15-payment-gateway-integration.md#152-payment-flow)
  - [15.3 Order state transitions during payment — pending, processing, payment_review](chapters/ch-15-payment-gateway-integration.md#153-order-state-transitions-during-payment)
  - [15.4 Redirect-based payment flow — 3DS, return URL, IPN/webhook handling](chapters/ch-15-payment-gateway-integration.md#154-redirect-based-payment-flow)
  - [15.5 Webhook/IPN processing — order synchronization, idempotent status updates](chapters/ch-15-payment-gateway-integration.md#155-webhookipn-processing)
  - [15.6 TELR & Iyzico integration patterns — lessons from real implementation](chapters/ch-15-payment-gateway-integration.md#156-telr-iyzico-integration-patterns)
  - [15.7 Payment extension config in `config.xml`, `payment.xml` — group, model, active flag](chapters/ch-15-payment-gateway-integration.md#157-payment-extension-config-in-configxml-paymentxml)

- [CH-16: Shipping API Integration](chapters/ch-16-shipping-api-integration.md)
  - [16.1 Magento carrier model — extending `AbstractCarrier`, implementing `collectRates()`](chapters/ch-16-shipping-api-integration.md#161-magento-carrier-model)
  - [16.2 `RateRequest` → `Result` → `Method` — rate request/response objects](chapters/ch-16-shipping-api-integration.md#162-raterequest-result-method)
  - [16.3 Label generation — creating shipments programmatically, track numbers](chapters/ch-16-shipping-api-integration.md#163-label-generation)
  - [16.4 Tracking updates — polling vs webhook, updating `sales_shipment_track`](chapters/ch-16-shipping-api-integration.md#164-tracking-updates)
  - [16.5 DHL & USPS integration lessons — rate limits, API auth, error handling](chapters/ch-16-shipping-api-integration.md#165-dhl-usps-integration-lessons)

- [CH-17: Multi-Source Inventory (MSI)](chapters/ch-17-multi-source-inventory-msi.md)
  - [17.1 MSI architecture — Sources, Stocks, Stock-Source links](chapters/ch-17-multi-source-inventory-msi.md#171-msi-architecture)
  - [17.2 Sales Channel → Stock → Source resolution chain](chapters/ch-17-multi-source-inventory-msi.md#172-sales-channel-stock-source-resolution-chain)
  - [17.3 MSI APIs — `SourceItemsSaveInterface`, `GetProductSalableQtyInterface`](chapters/ch-17-multi-source-inventory-msi.md#173-msi-apis)
  - [17.4 Custom stock algorithm — implementing `GetProductSalableQtyInterface`](chapters/ch-17-multi-source-inventory-msi.md#174-custom-stock-algorithm)
  - [17.5 MSI in checkout — reservation concept, `ReservationInterface`](chapters/ch-17-multi-source-inventory-msi.md#175-msi-in-checkout)
  - [17.6 Inventory sync with external system (Amazon) — MSI API update pattern](chapters/ch-17-multi-source-inventory-msi.md#176-inventory-sync-with-external-system-amazon)

- [CH-18: Frontend — Layout XML & Blocks](chapters/ch-18-frontend-layout-xml-blocks.md)
  - [18.1 Layout handles — page-specific, route-specific, custom handles](chapters/ch-18-frontend-layout-xml-blocks.md#181-layout-handles)
  - [18.2 Containers and blocks — `<container>`, `<block>`, hierarchy in layout XML](chapters/ch-18-frontend-layout-xml-blocks.md#182-containers-and-blocks)
  - [18.3 `referenceBlock`, `referenceContainer`, `move`, `remove` directives](chapters/ch-18-frontend-layout-xml-blocks.md#183-referenceblock-referencecontainer-move-remove-directives)
  - [18.4 Block PHP class — `_prepareLayout()`, `toHtml()`, `getChildHtml()`](chapters/ch-18-frontend-layout-xml-blocks.md#184-block-php-class)
  - [18.5 Block caching — `getCacheKeyInfo()`, `getCacheLifetime()`, cache tags in blocks](chapters/ch-18-frontend-layout-xml-blocks.md#185-block-caching)
  - [18.6 PHTML templates — escaping output, `$escaper`, XSS prevention](chapters/ch-18-frontend-layout-xml-blocks.md#186-phtml-templates)
  - [18.7 Template override — theme inheritance, `theme.xml`, `<parent>` in themes](chapters/ch-18-frontend-layout-xml-blocks.md#187-template-override)

- [CH-19: Frontend — Hyva Theme](chapters/ch-19-frontend-hyva-theme.md)
  - [19.1 Why Hyva exists — no RequireJS/KnockoutJS, AlpineJS + Tailwind CSS](chapters/ch-19-frontend-hyva-theme.md#191-why-hyva-exists)
  - [19.2 Hyva theme structure — difference from Luma, no `ui-component` overhead](chapters/ch-19-frontend-hyva-theme.md#192-hyva-theme-structure)
  - [19.3 AlpineJS in Hyva — `x-data`, `x-on`, `x-show`, `x-model`, component state](chapters/ch-19-frontend-hyva-theme.md#193-alpinejs-in-hyva)
  - [19.4 Hyva events system — `window.dispatchEvent`, `window.addEventListener` for inter-component communication](chapters/ch-19-frontend-hyva-theme.md#194-hyva-events-system)
  - [19.5 Tailwind CSS in Hyva — purging unused classes, custom config, JIT mode](chapters/ch-19-frontend-hyva-theme.md#195-tailwind-css-in-hyva)
  - [19.6 Hyva checkout — separate module, Alpine-driven multi-step, customization points](chapters/ch-19-frontend-hyva-theme.md#196-hyva-checkout)
  - [19.7 Overriding Hyva templates in a child theme — fallback resolution order](chapters/ch-19-frontend-hyva-theme.md#197-overriding-hyva-templates-in-a-child-theme)

- [CH-20: UI Components (Admin)](chapters/ch-20-ui-components-admin.md)
  - [20.1 UI component architecture — XML definition, PHP DataProvider, JS component](chapters/ch-20-ui-components-admin.md#201-ui-component-architecture)
  - [20.2 Admin listing (grid) — `listing`, `columns`, `filters`, `paging`, mass actions](chapters/ch-20-ui-components-admin.md#202-admin-listing-grid)
  - [20.3 Admin form — `form`, `fieldset`, `field`, custom element types](chapters/ch-20-ui-components-admin.md#203-admin-form)
  - [20.4 DataProvider class — `getDataSourceData()`, `addFilter()`, `getSearchResult()`](chapters/ch-20-ui-components-admin.md#204-dataprovider-class)
  - [20.5 Dynamic rows — variable-count fields in admin forms](chapters/ch-20-ui-components-admin.md#205-dynamic-rows)

- [CH-21: Performance Optimization](chapters/ch-21-performance-optimization.md)
  - [21.1 Magento modes — developer, production, default — impact on performance](chapters/ch-21-performance-optimization.md#211-magento-modes)
  - [21.2 Static content deploy — `setup:static-content:deploy`, strategies, parallel deployment](chapters/ch-21-performance-optimization.md#212-static-content-deploy)
  - [21.3 DI compilation — `setup:di:compile`, generated interceptors and factories](chapters/ch-21-performance-optimization.md#213-di-compilation)
  - [21.4 Varnish configuration — VCL file, grace mode, cache hit/miss headers](chapters/ch-21-performance-optimization.md#214-varnish-configuration)
  - [21.5 Redis optimization — session locking, `redis_cluster`, `compress_data`](chapters/ch-21-performance-optimization.md#215-redis-optimization)
  - [21.6 Database query optimization — slow query log, `EXPLAIN`, indexing DB columns](chapters/ch-21-performance-optimization.md#216-database-query-optimization)
  - [21.7 Magento profiler — `?profiler=1`, `var/log/` files, New Relic / Blackfire integration](chapters/ch-21-performance-optimization.md#217-magento-profiler)
  - [21.8 Image optimization — WebP, lazy loading, `<img>` in Hyva](chapters/ch-21-performance-optimization.md#218-image-optimization)
  - [21.9 JavaScript bundling — Hyva vs Luma approach, critical CSS, deferred loading](chapters/ch-21-performance-optimization.md#219-javascript-bundling)

- [CH-22: Search — Elasticsearch & OpenSearch](chapters/ch-22-search-elasticsearch-opensearch.md)
  - [22.1 Magento search adapter pattern — `SearchAdapterInterface`, query building](chapters/ch-22-search-elasticsearch-opensearch.md#221-magento-search-adapter-pattern)
  - [22.2 Catalog search indexer — what product data goes into ES index, field mapping](chapters/ch-22-search-elasticsearch-opensearch.md#222-catalog-search-indexer)
  - [22.3 Query DSL — `match`, `filter`, `bool`, `range`, aggregations for layered nav](chapters/ch-22-search-elasticsearch-opensearch.md#223-query-dsl)
  - [22.4 Search relevance — boosting, custom weights for product fields](chapters/ch-22-search-elasticsearch-opensearch.md#224-search-relevance)
  - [22.5 Index mapping customization — adding custom fields, keyword vs text, analyzers](chapters/ch-22-search-elasticsearch-opensearch.md#225-index-mapping-customization)
  - [22.6 Search synonyms, stop words, stemming — linguistic processing in Magento](chapters/ch-22-search-elasticsearch-opensearch.md#226-search-synonyms-stop-words-stemming)
  - [22.7 Switching search engine — OpenSearch vs Elasticsearch config in `env.php`](chapters/ch-22-search-elasticsearch-opensearch.md#227-switching-search-engine)

- [CH-23: AI & RAG-Based Search (Your Edge)](chapters/ch-23-ai-rag-based-search-your-edge.md)
  - [23.1 Embedding pipeline — product text → ONNX embedding model → vector → ES/OpenSearch index](chapters/ch-23-ai-rag-based-search-your-edge.md#231-embedding-pipeline)
  - [23.2 kNN vector search — approximate nearest neighbor, HNSW algorithm in ES](chapters/ch-23-ai-rag-based-search-your-edge.md#232-knn-vector-search)
  - [23.3 RAG pattern — retrieval-augmented generation, chunking strategy, context injection](chapters/ch-23-ai-rag-based-search-your-edge.md#233-rag-pattern)
  - [23.4 ChromaDB for semantic search — collection setup, distance metrics, metadata filtering](chapters/ch-23-ai-rag-based-search-your-edge.md#234-chromadb-for-semantic-search)
  - [23.5 Multimodal / image-based search — CLIP-style embeddings, image vector indexing](chapters/ch-23-ai-rag-based-search-your-edge.md#235-multimodal-image-based-search)
  - [23.6 Symfony AI Agent components — tool definitions, agent loop, LLM orchestration](chapters/ch-23-ai-rag-based-search-your-edge.md#236-symfony-ai-agent-components)
  - [23.7 AI agent with Magento tools — catalog search tool, inventory check tool, order creation tool](chapters/ch-23-ai-rag-based-search-your-edge.md#237-ai-agent-with-magento-tools)

- [CH-24: Security Best Practices](chapters/ch-24-security-best-practices.md)
  - [24.1 XSS prevention — `$escaper` in templates, `escapeHtml()`, `escapeUrl()`, `escapeJs()`](chapters/ch-24-security-best-practices.md#241-xss-prevention)
  - [24.2 CSRF protection — form keys, `FormKeyValidator`, REST API exceptions](chapters/ch-24-security-best-practices.md#242-csrf-protection)
  - [24.3 SQL injection prevention — parameterized queries in ResourceModel, no raw SQL](chapters/ch-24-security-best-practices.md#243-sql-injection-prevention)
  - [24.4 ACL and role-based access — `acl.xml`, `_isAllowed()`, resource IDs](chapters/ch-24-security-best-practices.md#244-acl-and-role-based-access)
  - [24.5 Sensitive data handling — no passwords in logs, encryption key, `env.php` security](chapters/ch-24-security-best-practices.md#245-sensitive-data-handling)
  - [24.6 Security patches — applying patches, Composer security advisories](chapters/ch-24-security-best-practices.md#246-security-patches)
  - [24.7 Admin security — two-factor authentication (2FA), custom admin URL, IP whitelist](chapters/ch-24-security-best-practices.md#247-admin-security)

- [CH-25: DevOps, CLI & Deployment](chapters/ch-25-devops-cli-deployment.md)
  - [25.1 Key `bin/magento` commands — setup, cache, indexer, module, cron commands](chapters/ch-25-devops-cli-deployment.md#251-key-binmagento-commands)
  - [25.2 Deployment pipeline — static deploy, DI compile, DB upgrade, cache flush order](chapters/ch-25-devops-cli-deployment.md#252-deployment-pipeline)
  - [25.3 Docker setup for Magento 2 — typical `docker-compose.yml`, services (nginx, php-fpm, mysql, redis, elasticsearch)](chapters/ch-25-devops-cli-deployment.md#253-docker-setup-for-magento-2)
  - [25.4 Zero-downtime deployment — maintenance mode, symlink strategy, pipeline steps](chapters/ch-25-devops-cli-deployment.md#254-zero-downtime-deployment)
  - [25.5 Adobe Commerce Cloud — cloud-specific config, `.magento.env.yaml`, pipelines](chapters/ch-25-devops-cli-deployment.md#255-adobe-commerce-cloud)
  - [25.6 Logging — `var/log/system.log`, `exception.log`, custom logger via `di.xml`](chapters/ch-25-devops-cli-deployment.md#256-logging)
  - [25.7 Magento cron setup — `crontab -e` entry, cron groups, `cron:run` command](chapters/ch-25-devops-cli-deployment.md#257-magento-cron-setup)

- [CH-26: Composer & Dependency Management](chapters/ch-26-composer-dependency-management.md)
  - [26.1 `composer.json` vs `composer.lock` — purpose, why `lock` must be committed](chapters/ch-26-composer-dependency-management.md#261-composerjson-vs-composerlock)
  - [26.2 Metapackages — how Magento uses them, `magento/product-community-edition`](chapters/ch-26-composer-dependency-management.md#262-metapackages)
  - [26.3 Installing / updating extensions — Marketplace, private repos, `composer require`](chapters/ch-26-composer-dependency-management.md#263-installing-updating-extensions)
  - [26.4 Autoloading — PSR-4 in Magento, `registration.php` role, generated autoload](chapters/ch-26-composer-dependency-management.md#264-autoloading)

- [CH-27: Magento 2.3 vs 2.4 vs Adobe Commerce](chapters/ch-27-magento-23-vs-24-vs-adobe-commerce.md)
  - [27.1 Magento 2.3 key features — declarative schema, async API, PWA Studio](chapters/ch-27-magento-23-vs-24-vs-adobe-commerce.md#271-magento-23-key-features)
  - [27.2 Magento 2.4 key changes — Elasticsearch mandatory, 2FA, PHP 8 support, improved GraphQL](chapters/ch-27-magento-23-vs-24-vs-adobe-commerce.md#272-magento-24-key-changes)
  - [27.3 Adobe Commerce (formerly Commerce) exclusive features — B2B module, Page Builder, Customer Segments, Staging & Preview](chapters/ch-27-magento-23-vs-24-vs-adobe-commerce.md#273-adobe-commerce-formerly-commerce-exclusive-features)
  - [27.4 B2B module — company accounts, shared catalogs, requisition lists, quick order](chapters/ch-27-magento-23-vs-24-vs-adobe-commerce.md#274-b2b-module)
  - [27.5 Open Source vs Adobe Commerce — licensing, feature comparison, when to recommend each](chapters/ch-27-magento-23-vs-24-vs-adobe-commerce.md#275-open-source-vs-adobe-commerce)

- [CH-28: Compliance & Tax Integrations](chapters/ch-28-compliance-tax-integrations.md)
  - [28.1 ZATCA (Saudi Arabia) e-invoicing — Phase 1 vs Phase 2, FATOORAH format, UBL XML](chapters/ch-28-compliance-tax-integrations.md#281-zatca-saudi-arabia-e-invoicing)
  - [28.2 VeriFactu (Spain) — invoice signing, tax agency submission, fiscal compliance](chapters/ch-28-compliance-tax-integrations.md#282-verifactu-spain)
  - [28.3 Tax calculation flow in Magento — `TaxCalculationInterface`, tax rules, rates, classes](chapters/ch-28-compliance-tax-integrations.md#283-tax-calculation-flow-in-magento)
  - [28.4 VAT validation — customer group switching on valid VAT, EU cross-border rules](chapters/ch-28-compliance-tax-integrations.md#284-vat-validation)
  - [28.5 International compliance lessons — regional API integration patterns, error handling](chapters/ch-28-compliance-tax-integrations.md#285-international-compliance-lessons)

- [CH-29: PHP & OOP Concepts for Magento](chapters/ch-29-php-oop-concepts-for-magento.md)
  - [29.1 PHP 8.x features relevant to Magento — named arguments, match expression, nullsafe operator, fibers](chapters/ch-29-php-oop-concepts-for-magento.md#291-php-8x-features-relevant-to-magento)
  - [29.2 Interfaces vs abstract classes — when Magento uses each and why](chapters/ch-29-php-oop-concepts-for-magento.md#292-interfaces-vs-abstract-classes)
  - [29.3 Traits in PHP — usage in Magento helpers and mixins](chapters/ch-29-php-oop-concepts-for-magento.md#293-traits-in-php)
  - [29.4 SOLID principles — how each applies to Magento module development](chapters/ch-29-php-oop-concepts-for-magento.md#294-solid-principles)
  - [29.5 Namespaces and PSR-4 autoloading — how Magento maps classes to files](chapters/ch-29-php-oop-concepts-for-magento.md#295-namespaces-and-psr-4-autoloading)
  - [29.6 PHP `__construct`, magic methods — `__get`, `__set`, `__call` in Magento DataObject](chapters/ch-29-php-oop-concepts-for-magento.md#296-php-__construct-magic-methods)
  - [29.7 Error handling — exceptions in Magento, `LocalizedException`, `NoSuchEntityException`](chapters/ch-29-php-oop-concepts-for-magento.md#297-error-handling)

- [CH-30: Scenario-Based Interview Questions](chapters/ch-30-scenario-based-interview-questions.md)
  - [30.1 "How would you add a custom attribute to the product and expose it via REST API?"](chapters/ch-30-scenario-based-interview-questions.md#301-how-would-you-add-a-custom-attribute-to-the-product-and-expose-it-via-rest-api)
  - [30.2 "How would you override a core Magento class?" — Plugin first, then Preference](chapters/ch-30-scenario-based-interview-questions.md#302-how-would-you-override-a-core-magento-class)
  - [30.3 "The site is slow after a deploy — how do you debug?" — Profiler, logs, cache, indexers](chapters/ch-30-scenario-based-interview-questions.md#303-the-site-is-slow-after-a-deploy)
  - [30.4 "Design an inventory sync system between Amazon and Magento" — Queue, MSI, idempotency](chapters/ch-30-scenario-based-interview-questions.md#304-design-an-inventory-sync-system-between-amazon-and-magento)
  - [30.5 "How would you create a custom payment gateway?" — Redirect flow, webhook, order sync](chapters/ch-30-scenario-based-interview-questions.md#305-how-would-you-create-a-custom-payment-gateway)
  - [30.6 "How would you implement a custom shipping carrier?" — `AbstractCarrier`, `collectRates()`](chapters/ch-30-scenario-based-interview-questions.md#306-how-would-you-implement-a-custom-shipping-carrier)
  - [30.7 "How would you add a new step to the checkout?" — Hyva checkout customization, step component](chapters/ch-30-scenario-based-interview-questions.md#307-how-would-you-add-a-new-step-to-the-checkout)
  - [30.8 "How would you build a semantic product search?" — ES embedding, kNN, RAG pipeline](chapters/ch-30-scenario-based-interview-questions.md#308-how-would-you-build-a-semantic-product-search)
  - [30.9 "How do you prevent a plugin from running in a specific area?" — Area check in plugin logic](chapters/ch-30-scenario-based-interview-questions.md#309-how-do-you-prevent-a-plugin-from-running-in-a-specific-area)
  - [30.10 "How would you debug a cron job that is not running?" — `cron_schedule` table, group config, log check](chapters/ch-30-scenario-based-interview-questions.md#3010-how-would-you-debug-a-cron-job-that-is-not-running)

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

