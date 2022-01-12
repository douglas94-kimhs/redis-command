# redis-command
# Reference : https://www.youtube.com/watch?v=0wqZd3zwh7Y&t=2s
1. Redis-client 명령어
   String 입력/조회
      set name Shabbir  ==> get name
      set email email@domain.com = > get email  / getrange email 0 4
      mset lang English technology redis / mget lang technology
      strlen lang
      set name "Daily Code Buffer"
      get name
      set count 1
      get count
      incr count
      incrby count 10
      decr count
      set a 1
      expire a 10 (10초 설정)
      setex b 10 ttl_test
      keys *
      flushall 
      
      ## List ##
      lpush country india
      lpush country usa
      lrange country 0 -1 (lpush 왼쪽부터 추가, rpush 오른쪽 추가)
      llen country
      lpop / rpop
      lset country 0 Germany
      lindex country 2
      
      ## Set ##
      sadd technology java
      sadd technology redis, nodejs, aws
      smembers technology
      scard technology
      sismember technology java
      sadd frontend redis, nodejs, aws
      sdiff technology frontend
      sdiffstore newset technology frontend
      sinter frontend technology
      
      ## hash ##
      hkeys myhash
      hvals myhash
      hgetall myhash
      hexists
      hlen
      hset
      hlen
      hmset
      hmget
      
      
      
      
      
      
      
