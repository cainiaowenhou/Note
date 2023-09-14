## 排序

- Arrays.sort(arr);
- Arrays.sort(arr, Collections.reverseOrder());
- arraylist.sort();
## String
- 数组转换成字符串：list.toString();
- 字符串切片：str.substring(startIdx, endIdx);
- 字符串转数字： Integer.parseInt(str)/Integer.valueOf(str);
- 字符串数组：str.split(", ");
- length:数组
- length()、size()::泛型
- 转换成List: String[] strArr = data.split(","); List<String> dataList = new LinkedList<String>(Arrays.asList(strArr));
## 队列
- 初始化：Queue<Integer> queue = new LinkedList<Integer>();
- 入队：queue.offer()
- 出队：queue.poll()
- 初始化：Deque<Integer> queue = new LinkedList<Integer>();
- 入队：queue.offerFirst(); queue.offerLast();
- 出队：queue.pollFirst(); queue.pollLast();
## 哈希表
- 初始化：HashMap<Integer, String> map = new HashMap<Integer, String>();
- 添加k-v: map.put(key, value);
- 获取v : map.get(key);
- 删除：map.remove(key);
- 迭代： for(Integer i: map.keySet()){}
- 判空：map.isEmpty()
- 判key: map.containsKey(key)

## 最大值最小值
- Long.MIN_VALUE
- Long.MAX_VALUE
