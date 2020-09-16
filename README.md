# Notebook
笔记
---

## kafka
  + 生产者
  ~~~
  producer = KafkaProducer(value_serializer=lambda v: json.dumps(v).encode('gbk'),
                             bootstrap_servers=['192.168.20.80:9092', '192.168.20.81:9092', '192.168.20.82:9092',
                                                '192.168.20.83:9092', '192.168.20.84:9092'])

 producer.send('test_0914', data_kfk) #定义topic名称
 producer.close()
 ~~~
 
  + 消费者
    
