# Magento 2 Interview Preparation Roadmap
### Nitish Kumar Upadhyay — 3+ Years Experience | Adobe Certified Developer

---

## 📋 Progress Tracker

| Chapter | Topics | Status |
|---------|--------|--------|
| CH-01: Architecture & Request Lifecycle | 8 topics | [ ] |
| CH-02: Dependency Injection & Object Manager | 7 topics | [ ] |
| CH-03: Module Development | 10 topics | [ ] |
| CH-04: Plugin System & Interceptors | 6 topics | [ ] |
| CH-05: Events & Observers | 5 topics | [ ] |
| CH-06: Design Patterns in Magento 2 | 10 topics | [ ] |
| CH-07: Service Contracts & Repositories | 7 topics | [ ] |
| CH-08: Database, ORM & EAV Model | 9 topics | [ ] |
| CH-09: Declarative Schema & Data Patches | 6 topics | [ ] |
| CH-10: Caching System | 8 topics | [ ] |
| CH-11: Indexing System | 7 topics | [ ] |
| CH-12: REST API & Web API | 8 topics | [ ] |
| CH-13: GraphQL API | 7 topics | [ ] |
| CH-14: Message Queues & Async Processing | 6 topics | [ ] |
| CH-15: Payment Gateway Integration | 7 topics | [ ] |
| CH-16: Shipping API Integration | 5 topics | [ ] |
| CH-17: Multi-Source Inventory (MSI) | 6 topics | [ ] |
| CH-18: Frontend — Layout XML & Blocks | 7 topics | [ ] |
| CH-19: Frontend — Hyva Theme | 7 topics | [ ] |
| CH-20: UI Components (Admin) | 5 topics | [ ] |
| CH-21: Performance Optimization | 9 topics | [ ] |
| CH-22: Search — Elasticsearch & OpenSearch | 7 topics | [ ] |
| CH-23: AI & RAG-Based Search (Your Edge) | 7 topics | [ ] |
| CH-24: Security Best Practices | 7 topics | [ ] |
| CH-25: DevOps, CLI & Deployment | 7 topics | [ ] |
| CH-26: Composer & Dependency Management | 4 topics | [ ] |
| CH-27: Magento 2.3 vs 2.4 vs Adobe Commerce | 5 topics | [ ] |
| CH-28: Compliance & Tax Integrations | 5 topics | [ ] |
| CH-29: PHP & OOP Concepts for Magento | 7 topics | [ ] |
| CH-30: Scenario-Based Interview Questions | 10 topics | [ ] |

---

## CH-01: Architecture & Request Lifecycle

- [ ] **1.1** Magento 2 overall architecture overview — areas, layers, components
- [ ] **1.2** Application areas — `frontend`, `adminhtml`, `crontab`, `webapi_rest`, `graphql`, `doc`
- [ ] **1.3** Request lifecycle — `index.php` → Bootstrap → App → FrontController → Router → Controller
- [ ] **1.4** Router types — standard, admin, CMS, default (404)
- [ ] **1.5** Controller anatomy — `execute()`, `ResultFactory`, redirect vs page vs JSON response
- [ ] **1.6** Action URL structure — `frontName/controller/action`
- [ ] **1.7** Magento directory structure — `app/`, `vendor/`, `pub/`, `var/`, `generated/`
- [ ] **1.8** Module file structure — `registration.php`, `module.xml`, `etc/`, `Block/`, `Controller/`, `Model/`, `view/`

---

## CH-02: Dependency Injection & Object Manager

- [ ] **2.1** What is Dependency Injection — constructor vs method vs property injection
- [ ] **2.2** `di.xml` configuration — `<preference>`, `<type>`, `<arguments>`, `<virtualType>`
- [ ] **2.3** Object Manager — role, why not to use it directly in production code
- [ ] **2.4** Shared vs non-shared instances — singletons and factories
- [ ] **2.5** Factory classes — when and why to use `SomeClassFactory`
- [ ] **2.6** Proxy classes — lazy-loading heavy dependencies, `SomeClassProxy`
- [ ] **2.7** Virtual types — reusing class configuration without creating new classes

---

## CH-03: Module Development

- [ ] **3.1** Creating a module from scratch — `registration.php`, `module.xml`, `composer.json`
- [ ] **3.2** Module load order — `<sequence>` in `module.xml`, dependency resolution
- [ ] **3.3** Module enable/disable — `bin/magento module:enable`, `module_setup` table
- [ ] **3.4** Creating a custom controller — frontend and admin routing
- [ ] **3.5** Creating a custom admin grid with UI component
- [ ] **3.6** Custom system configuration — `system.xml`, `config.xml`, `acl.xml`
- [ ] **3.7** Adding custom attributes to products, customers, orders
- [ ] **3.8** Extension attributes — `extension_attributes.xml`, join directives
- [ ] **3.9** Custom cron job — `crontab.xml`, cron groups, schedule expression
- [ ] **3.10** Custom CLI command — `di.xml` registration, `InputInterface`, `OutputInterface`

---

## CH-04: Plugin System & Interceptors

- [ ] **4.1** Plugin types — Before, Around, After — purpose and signature of each
- [ ] **4.2** Around plugin — `$proceed()` call, skipping original method, wrapping logic
- [ ] **4.3** Plugin limitations — final classes, static methods, non-public methods, `__construct`
- [ ] **4.4** Plugin sort order — `sortOrder` attribute and conflict resolution
- [ ] **4.5** Plugin vs Preference vs Observer — when to choose which
- [ ] **4.6** Can you plugin a plugin? — generated interceptor class explanation

---

## CH-05: Events & Observers

- [ ] **5.1** Event-Observer pattern — `events.xml` structure, `instance` and `method`
- [ ] **5.2** Area-specific vs global event registration
- [ ] **5.3** Dispatching custom events — `EventManager::dispatch()`, `DataObject`
- [ ] **5.4** Key Magento events — `sales_order_place_after`, `customer_register_success`, `catalog_product_save_after`
- [ ] **5.5** Observer best practices — keeping observers lightweight, no heavy DB operations

---

## CH-06: Design Patterns in Magento 2

- [ ] **6.1** Singleton pattern — shared object instances in DI container
- [ ] **6.2** Factory pattern — object creation via generated factory classes
- [ ] **6.3** Repository pattern — data access abstraction over ResourceModels
- [ ] **6.4** Service Contract pattern — interfaces as stable API layer
- [ ] **6.5** Observer / Event pattern — decoupled event-driven communication
- [ ] **6.6** Plugin / Interceptor pattern — method-level AOP without inheritance
- [ ] **6.7** Proxy pattern — deferred object initialization for performance
- [ ] **6.8** Strategy pattern — swappable algorithms (e.g. shipping rate carriers)
- [ ] **6.9** Decorator pattern — wrapping objects to add behavior
- [ ] **6.10** Composite pattern — tree structures (e.g. category tree, layout blocks)

---

## CH-07: Service Contracts & Repositories

- [ ] **7.1** What are service contracts — interfaces in `Api/` folder, why they matter
- [ ] **7.2** Data interfaces (DTOs) — `Api/Data/`, difference from Model objects
- [ ] **7.3** Repository interface methods — `getById()`, `save()`, `delete()`, `getList()`
- [ ] **7.4** `SearchCriteriaInterface` — FilterGroup, Filter, SortOrder, page size
- [ ] **7.5** `SearchResultsInterface` — returning paginated lists from `getList()`
- [ ] **7.6** Never pass Model across service layer — use Data interfaces instead
- [ ] **7.7** Custom repository implementation — ResourceModel usage inside repository

---

## CH-08: Database, ORM & EAV Model

- [ ] **8.1** EAV model — what it is, why Magento uses it for products and customers
- [ ] **8.2** EAV tables — `eav_entity_type`, `catalog_product_entity`, `_varchar`, `_int`, `_decimal`, `_datetime`, `_text`
- [ ] **8.3** Flat model vs EAV — performance difference, flat catalog tables
- [ ] **8.4** ResourceModel — extending `AbstractDb`, `_init()`, `_construct()`
- [ ] **8.5** Collection — `addFieldToFilter()`, `addAttributeToFilter()`, `getSelect()`
- [ ] **8.6** Joining tables in a collection — `getSelect()->join()`, `joinLeft()`
- [ ] **8.7** `load()` on Model vs using Repository — when each is appropriate
- [ ] **8.8** Custom attribute backend types — `varchar`, `int`, `decimal`, `text`, `datetime`
- [ ] **8.9** Source models, backend models, frontend models for custom attributes

---

## CH-09: Declarative Schema & Data Patches

- [ ] **9.1** Declarative schema — `db_schema.xml` vs old `InstallSchema` / `UpgradeSchema`
- [ ] **9.2** `db_schema_whitelist.json` — why it's generated and what it controls
- [ ] **9.3** Data patches — `DataPatchInterface`, `getDependencies()`, `getAliases()`
- [ ] **9.4** Schema patches — `SchemaPatchInterface` for structural changes
- [ ] **9.5** Revertable patches — implementing `revert()` method
- [ ] **9.6** Patch execution tracking — `patch_list` table, preventing re-runs

---

## CH-10: Caching System

- [ ] **10.1** Magento cache types — `config`, `layout`, `block_html`, `full_page`, `collections`, `eav`, `translate`, `reflection`
- [ ] **10.2** Cache backend — file system vs Redis — configuration in `env.php`
- [ ] **10.3** Full Page Cache (FPC) — built-in vs Varnish, how it works
- [ ] **10.4** Hole-punching with ESI (Edge Side Includes) — private blocks in cached pages
- [ ] **10.5** Cache tags — how Magento tags blocks, `getCacheKeyInfo()`, `getCacheTags()`
- [ ] **10.6** Selective cache invalidation — `cache:clean` vs `cache:flush`, `clean()` with tags
- [ ] **10.7** Custom cache type — implementing `FrontendInterface`, registering in `di.xml`
- [ ] **10.8** Redis for sessions — `session.save` config, session locking considerations

---

## CH-11: Indexing System

- [ ] **11.1** What indexers do — why Magento needs them (EAV to flat, price calculation, search)
- [ ] **11.2** Index modes — `realtime` vs `schedule`, when to use each
- [ ] **11.3** Key indexers — `catalog_product_price`, `catalogsearch_fulltext`, `cataloginventory_stock`, `catalog_category_product`
- [ ] **11.4** Mview (materialized view) — how schedule mode tracks incremental changes
- [ ] **11.5** Custom indexer — implementing `IndexerInterface`, registering in `indexer.xml`
- [ ] **11.6** `bin/magento indexer:reindex` — full vs partial reindex
- [ ] **11.7** Indexer performance — large catalog considerations, partial indexing triggers

---

## CH-12: REST API & Web API

- [ ] **12.1** `webapi.xml` — route, HTTP method, service interface method, resource ACL
- [ ] **12.2** Auth methods — admin token, customer token, OAuth 1.0a, guest
- [ ] **12.3** Exposing custom endpoints — service contract → `webapi.xml` → auto-routing
- [ ] **12.4** `SearchCriteria` in REST — filter groups, filters, sorting, pagination via URL params
- [ ] **12.5** Async REST API — `async/bulk/` prefix, queue-based processing
- [ ] **12.6** Bulk API operations — `V1/bulk` endpoint, status tracking
- [ ] **12.7** REST API versioning — `/V1/`, `/V2/` — backward compatibility contract
- [ ] **12.8** Amazon-to-Magento inventory sync — SP-API integration, queue pattern, idempotency

---

## CH-13: GraphQL API

- [ ] **13.1** `schema.graphqls` — type definitions, queries, mutations, interfaces
- [ ] **13.2** Resolver classes — implementing `ResolverInterface`, returning array
- [ ] **13.3** Context object — store scope, customer identity, authorization
- [ ] **13.4** Extending existing Magento GraphQL types — `@resolver`, `@doc` directives
- [ ] **13.5** Custom query vs custom mutation — when to use each
- [ ] **13.6** N+1 problem in GraphQL — batching with `BatchContractInterface`, deferred resolvers
- [ ] **13.7** GraphQL caching — cache resolution, `@cache` directive, Varnish + GraphQL

---

## CH-14: Message Queues & Async Processing

- [ ] **14.1** Queue configuration files — `queue.xml`, `communication.xml`, `topology.xml`
- [ ] **14.2** Publisher → Exchange → Queue → Consumer flow
- [ ] **14.3** RabbitMQ vs MySQL queue — when to use each
- [ ] **14.4** Consumer management — `bin/magento queue:consumers:start`, supervisor daemon
- [ ] **14.5** Dead letter queues — failed message handling, retry strategies
- [ ] **14.6** When to use message queues vs synchronous processing — trade-off decisions

---

## CH-15: Payment Gateway Integration

- [ ] **15.1** Payment method interface — `MethodInterface` vs `AbstractMethod` (legacy)
- [ ] **15.2** Payment flow — `authorize()`, `capture()`, `void()`, `refund()`, `cancel()`
- [ ] **15.3** Order state transitions during payment — pending, processing, payment_review
- [ ] **15.4** Redirect-based payment flow — 3DS, return URL, IPN/webhook handling
- [ ] **15.5** Webhook/IPN processing — order synchronization, idempotent status updates
- [ ] **15.6** TELR & Iyzico integration patterns — lessons from real implementation
- [ ] **15.7** Payment extension config in `config.xml`, `payment.xml` — group, model, active flag

---

## CH-16: Shipping API Integration

- [ ] **16.1** Magento carrier model — extending `AbstractCarrier`, implementing `collectRates()`
- [ ] **16.2** `RateRequest` → `Result` → `Method` — rate request/response objects
- [ ] **16.3** Label generation — creating shipments programmatically, track numbers
- [ ] **16.4** Tracking updates — polling vs webhook, updating `sales_shipment_track`
- [ ] **16.5** DHL & USPS integration lessons — rate limits, API auth, error handling

---

## CH-17: Multi-Source Inventory (MSI)

- [ ] **17.1** MSI architecture — Sources, Stocks, Stock-Source links
- [ ] **17.2** Sales Channel → Stock → Source resolution chain
- [ ] **17.3** MSI APIs — `SourceItemsSaveInterface`, `GetProductSalableQtyInterface`
- [ ] **17.4** Custom stock algorithm — implementing `GetProductSalableQtyInterface`
- [ ] **17.5** MSI in checkout — reservation concept, `ReservationInterface`
- [ ] **17.6** Inventory sync with external system (Amazon) — MSI API update pattern

---

## CH-18: Frontend — Layout XML & Blocks

- [ ] **18.1** Layout handles — page-specific, route-specific, custom handles
- [ ] **18.2** Containers and blocks — `<container>`, `<block>`, hierarchy in layout XML
- [ ] **18.3** `referenceBlock`, `referenceContainer`, `move`, `remove` directives
- [ ] **18.4** Block PHP class — `_prepareLayout()`, `toHtml()`, `getChildHtml()`
- [ ] **18.5** Block caching — `getCacheKeyInfo()`, `getCacheLifetime()`, cache tags in blocks
- [ ] **18.6** PHTML templates — escaping output, `$escaper`, XSS prevention
- [ ] **18.7** Template override — theme inheritance, `theme.xml`, `<parent>` in themes

---

## CH-19: Frontend — Hyva Theme

- [ ] **19.1** Why Hyva exists — no RequireJS/KnockoutJS, AlpineJS + Tailwind CSS
- [ ] **19.2** Hyva theme structure — difference from Luma, no `ui-component` overhead
- [ ] **19.3** AlpineJS in Hyva — `x-data`, `x-on`, `x-show`, `x-model`, component state
- [ ] **19.4** Hyva events system — `window.dispatchEvent`, `window.addEventListener` for inter-component communication
- [ ] **19.5** Tailwind CSS in Hyva — purging unused classes, custom config, JIT mode
- [ ] **19.6** Hyva checkout — separate module, Alpine-driven multi-step, customization points
- [ ] **19.7** Overriding Hyva templates in a child theme — fallback resolution order

---

## CH-20: UI Components (Admin)

- [ ] **20.1** UI component architecture — XML definition, PHP DataProvider, JS component
- [ ] **20.2** Admin listing (grid) — `listing`, `columns`, `filters`, `paging`, mass actions
- [ ] **20.3** Admin form — `form`, `fieldset`, `field`, custom element types
- [ ] **20.4** DataProvider class — `getDataSourceData()`, `addFilter()`, `getSearchResult()`
- [ ] **20.5** Dynamic rows — variable-count fields in admin forms

---

## CH-21: Performance Optimization

- [ ] **21.1** Magento modes — developer, production, default — impact on performance
- [ ] **21.2** Static content deploy — `setup:static-content:deploy`, strategies, parallel deployment
- [ ] **21.3** DI compilation — `setup:di:compile`, generated interceptors and factories
- [ ] **21.4** Varnish configuration — VCL file, grace mode, cache hit/miss headers
- [ ] **21.5** Redis optimization — session locking, `redis_cluster`, `compress_data`
- [ ] **21.6** Database query optimization — slow query log, `EXPLAIN`, indexing DB columns
- [ ] **21.7** Magento profiler — `?profiler=1`, `var/log/` files, New Relic / Blackfire integration
- [ ] **21.8** Image optimization — WebP, lazy loading, `<img>` in Hyva
- [ ] **21.9** JavaScript bundling — Hyva vs Luma approach, critical CSS, deferred loading

---

## CH-22: Search — Elasticsearch & OpenSearch

- [ ] **22.1** Magento search adapter pattern — `SearchAdapterInterface`, query building
- [ ] **22.2** Catalog search indexer — what product data goes into ES index, field mapping
- [ ] **22.3** Query DSL — `match`, `filter`, `bool`, `range`, aggregations for layered nav
- [ ] **22.4** Search relevance — boosting, custom weights for product fields
- [ ] **22.5** Index mapping customization — adding custom fields, keyword vs text, analyzers
- [ ] **22.6** Search synonyms, stop words, stemming — linguistic processing in Magento
- [ ] **22.7** Switching search engine — OpenSearch vs Elasticsearch config in `env.php`

---

## CH-23: AI & RAG-Based Search (Your Edge)

- [ ] **23.1** Embedding pipeline — product text → ONNX embedding model → vector → ES/OpenSearch index
- [ ] **23.2** kNN vector search — approximate nearest neighbor, HNSW algorithm in ES
- [ ] **23.3** RAG pattern — retrieval-augmented generation, chunking strategy, context injection
- [ ] **23.4** ChromaDB for semantic search — collection setup, distance metrics, metadata filtering
- [ ] **23.5** Multimodal / image-based search — CLIP-style embeddings, image vector indexing
- [ ] **23.6** Symfony AI Agent components — tool definitions, agent loop, LLM orchestration
- [ ] **23.7** AI agent with Magento tools — catalog search tool, inventory check tool, order creation tool

---

## CH-24: Security Best Practices

- [ ] **24.1** XSS prevention — `$escaper` in templates, `escapeHtml()`, `escapeUrl()`, `escapeJs()`
- [ ] **24.2** CSRF protection — form keys, `FormKeyValidator`, REST API exceptions
- [ ] **24.3** SQL injection prevention — parameterized queries in ResourceModel, no raw SQL
- [ ] **24.4** ACL and role-based access — `acl.xml`, `_isAllowed()`, resource IDs
- [ ] **24.5** Sensitive data handling — no passwords in logs, encryption key, `env.php` security
- [ ] **24.6** Security patches — applying patches, Composer security advisories
- [ ] **24.7** Admin security — two-factor authentication (2FA), custom admin URL, IP whitelist

---

## CH-25: DevOps, CLI & Deployment

- [ ] **25.1** Key `bin/magento` commands — setup, cache, indexer, module, cron commands
- [ ] **25.2** Deployment pipeline — static deploy, DI compile, DB upgrade, cache flush order
- [ ] **25.3** Docker setup for Magento 2 — typical `docker-compose.yml`, services (nginx, php-fpm, mysql, redis, elasticsearch)
- [ ] **25.4** Zero-downtime deployment — maintenance mode, symlink strategy, pipeline steps
- [ ] **25.5** Adobe Commerce Cloud — cloud-specific config, `.magento.env.yaml`, pipelines
- [ ] **25.6** Logging — `var/log/system.log`, `exception.log`, custom logger via `di.xml`
- [ ] **25.7** Magento cron setup — `crontab -e` entry, cron groups, `cron:run` command

---

## CH-26: Composer & Dependency Management

- [ ] **26.1** `composer.json` vs `composer.lock` — purpose, why `lock` must be committed
- [ ] **26.2** Metapackages — how Magento uses them, `magento/product-community-edition`
- [ ] **26.3** Installing / updating extensions — Marketplace, private repos, `composer require`
- [ ] **26.4** Autoloading — PSR-4 in Magento, `registration.php` role, generated autoload

---

## CH-27: Magento 2.3 vs 2.4 vs Adobe Commerce

- [ ] **27.1** Magento 2.3 key features — declarative schema, async API, PWA Studio
- [ ] **27.2** Magento 2.4 key changes — Elasticsearch mandatory, 2FA, PHP 8 support, improved GraphQL
- [ ] **27.3** Adobe Commerce (formerly Commerce) exclusive features — B2B module, Page Builder, Customer Segments, Staging & Preview
- [ ] **27.4** B2B module — company accounts, shared catalogs, requisition lists, quick order
- [ ] **27.5** Open Source vs Adobe Commerce — licensing, feature comparison, when to recommend each

---

## CH-28: Compliance & Tax Integrations

- [ ] **28.1** ZATCA (Saudi Arabia) e-invoicing — Phase 1 vs Phase 2, FATOORAH format, UBL XML
- [ ] **28.2** VeriFactu (Spain) — invoice signing, tax agency submission, fiscal compliance
- [ ] **28.3** Tax calculation flow in Magento — `TaxCalculationInterface`, tax rules, rates, classes
- [ ] **28.4** VAT validation — customer group switching on valid VAT, EU cross-border rules
- [ ] **28.5** International compliance lessons — regional API integration patterns, error handling

---

## CH-29: PHP & OOP Concepts for Magento

- [ ] **29.1** PHP 8.x features relevant to Magento — named arguments, match expression, nullsafe operator, fibers
- [ ] **29.2** Interfaces vs abstract classes — when Magento uses each and why
- [ ] **29.3** Traits in PHP — usage in Magento helpers and mixins
- [ ] **29.4** SOLID principles — how each applies to Magento module development
- [ ] **29.5** Namespaces and PSR-4 autoloading — how Magento maps classes to files
- [ ] **29.6** PHP `__construct`, magic methods — `__get`, `__set`, `__call` in Magento DataObject
- [ ] **29.7** Error handling — exceptions in Magento, `LocalizedException`, `NoSuchEntityException`

---

## CH-30: Scenario-Based Interview Questions

- [ ] **30.1** "How would you add a custom attribute to the product and expose it via REST API?"
- [ ] **30.2** "How would you override a core Magento class?" — Plugin first, then Preference
- [ ] **30.3** "The site is slow after a deploy — how do you debug?" — Profiler, logs, cache, indexers
- [ ] **30.4** "Design an inventory sync system between Amazon and Magento" — Queue, MSI, idempotency
- [ ] **30.5** "How would you create a custom payment gateway?" — Redirect flow, webhook, order sync
- [ ] **30.6** "How would you implement a custom shipping carrier?" — `AbstractCarrier`, `collectRates()`
- [ ] **30.7** "How would you add a new step to the checkout?" — Hyva checkout customization, step component
- [ ] **30.8** "How would you build a semantic product search?" — ES embedding, kNN, RAG pipeline
- [ ] **30.9** "How do you prevent a plugin from running in a specific area?" — Area check in plugin logic
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