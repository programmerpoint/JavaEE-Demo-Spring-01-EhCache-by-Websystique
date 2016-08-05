#JavaEE_Demo_Spring_01_EhCache

##Based on:

http://websystique.com/spring/spring-4-cache-tutorial-with-ehcache/

###Caching Annotations

    @Cacheable : triggers cache population
    @CacheEvict : triggers cache eviction
    @CachePut : updates the cache without interfering with the method execution
    @Caching : regroups multiple cache operations to be applied on a method
    @CacheConfig : shares some common cache-related settings at class-level
    @EnableCaching : Configuration level annotation which enables Caching


###Getting Started:

1.  Add @EnableCaching AppConfig.java
2.  Create resources/ehcache.xml
3.  Add @Cacheable("products") in ProductServiceImpl.java public Product getByName(String name){};
4.  Add @CacheEvict(value = "products", allEntries = true) to clear cache
