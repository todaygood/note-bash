# bash中的遍历

参见： https://www.cyberciti.biz/faq/unix-linux-iterate-over-a-variable-range-of-numbers-in-bash/



遍历一个范围

```bash
for i in {1..5}
do
   echo "$i"
done

```

遍历一个范围2

```bash
START=1
END=5
echo "Countdown"
 
for (( c=$START; c<=$END; c++ ))
do
    echo -n "$c "
    sleep 1
done
```





遍历数组

```bash
#!/bin/bash
 
## define an array with three items ##
arrayname=( Dell HP Oracle )
 
## get item count using ${arrayname[@]} ##
for m in "${arrayname[@]}"
do
  echo "${m}"
  # do something on $m #
done
```
