# re


|成员函数|函数描述/介绍|
|:------|:--------|
 | [re.Compile](#recompile) | 编译正则 |
 | [re.CompilePOSIX](#recompileposix) |  |
 | [re.ExtractEmail](#reextractemail) | 从字符串中提取 email |
 | [re.ExtractHostPort](#reextracthostport) | 从结果中提取 `host:port` |
 | [re.ExtractIP](#reextractip) | 从内容中提取 IP 地址 |
 | [re.ExtractIPv4](#reextractipv4) | 从内容中提取 IPv4 地址 |
 | [re.ExtractIPv6](#reextractipv6) | 从内容中提取 IPv6 地址 |
 | [re.ExtractMac](#reextractmac) | 从字符串中提取可用的 Mac 地址 |
 | [re.ExtractPath](#reextractpath) | 从内容中提取路径 |
 | [re.ExtractTTY](#reextracttty) | 从内容中提取 TTY 内容 |
 | [re.ExtractURL](#reextracturl) | 从内容中提取 URL |
 | [re.Find](#refind) | 匹配并提取数据中符合正则的数据 |
 | [re.FindAll](#refindall) | 提取所有正则匹配到的数据 |
 | [re.FindAllIndex](#refindallindex) | 提取匹配到的数据的索引（起止位置） |
 | [re.FindGroup](#refindgroup) |  |
 | [re.FindGroupAll](#refindgroupall) |  |
 | [re.FindIndex](#refindindex) | 提取匹配到的数据索引位置（起止位置） |
 | [re.FindSubmatch](#refindsubmatch) | 正则匹配提取带分组的数据（只匹配一个） |
 | [re.FindSubmatchAll](#refindsubmatchall) | 正则匹配提取带分组的数据（匹配全部） |
 | [re.FindSubmatchAllIndex](#refindsubmatchallindex) | 匹配并提取分组带索引（起止位置） |
 | [re.FindSubmatchIndex](#refindsubmatchindex) | 只匹配并提取第一组的分组带索引（起止位置） |
 | [re.Grok](#regrok) | 从内容中按照 Grok 规则提取数据 |
 | [re.Match](#rematch) |  |
 | [re.MustCompile](#remustcompile) | 编译正则，如果编译失败则 Panic |
 | [re.MustCompilePOSIX](#remustcompileposix) | 编译正则 POSIX 模式，编译失败则 Panic |
 | [re.QuoteMeta](#requotemeta) | 把正则保留字符进行转义 |
 | [re.ReplaceAll](#rereplaceall) | 整体批量替换 |
 | [re.ReplaceAllWithFunc](#rereplaceallwithfunc) | 正则批量替换数据（使用函数处理匹配结果） |




 



## 函数定义

### re.Compile

编译正则

#### 详细描述



#### 定义：

`Compile(string) (*regexp.Regexp, error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| regexpStr | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `*regexp.Regexp` |   |
| r1 | `error` |   |


 
### re.CompilePOSIX



#### 详细描述

编译正则（同 Golang `regexp.CompilePOSIX`）

#### 定义：

`CompilePOSIX(string) (*regexp.Regexp, error)`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| regexpStr | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `*regexp.Regexp` |   |
| r1 | `error` |   |


 
### re.ExtractEmail

从字符串中提取 email

#### 详细描述



#### 定义：

`ExtractEmail(i any) []string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| emails | `[]string` |   |


 
### re.ExtractHostPort

从结果中提取 `host:port`

#### 详细描述



#### 定义：

`ExtractHostPort(i any) []string  doc:HOSTPORT`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| hostPorts | `[]string` |   |


 
### re.ExtractIP

从内容中提取 IP 地址

#### 详细描述



#### 定义：

`ExtractIP(i any) []string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| ipAddrs | `[]string` |   |


 
### re.ExtractIPv4

从内容中提取 IPv4 地址

#### 详细描述



#### 定义：

`ExtractIPv4(i any) []string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| ipAddrs | `[]string` |   |


 
### re.ExtractIPv6

从内容中提取 IPv6 地址

#### 详细描述



#### 定义：

`ExtractIPv6(i any) []string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| ipAddrs | `[]string` |   |


 
### re.ExtractMac

从字符串中提取可用的 Mac 地址

#### 详细描述



#### 定义：

`ExtractMac(i any) []string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| macAddrs | `[]string` |   |


 
### re.ExtractPath

从内容中提取路径

#### 详细描述



#### 定义：

`ExtractPath(i any) []string  doc:PATHPARAM`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| paths | `[]string` |   |


 
### re.ExtractTTY

从内容中提取 TTY 内容

#### 详细描述



#### 定义：

`ExtractTTY(i any) []string  doc:TTY`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| ttys | `[]string` |   |


 
### re.ExtractURL

从内容中提取 URL

#### 详细描述



#### 定义：

`ExtractURL(i any) []string  doc:URL`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `[]byte|string|io.Reader|any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| urls | `[]string` |   |


 
### re.Find

匹配并提取数据中符合正则的数据

#### 详细描述



#### 定义：

`Find(origin any, re string) string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| result | `string` |   |


 
### re.FindAll

提取所有正则匹配到的数据

#### 详细描述



#### 定义：

`FindAll(origin any, re string) []string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| results | `[]string` |   |


 
### re.FindAllIndex

提取匹配到的数据的索引（起止位置）

#### 详细描述



#### 定义：

`FindAllIndex(origin any, re string) [][]int`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| indexes | `[][start: int, end: int]` |   |


 
### re.FindGroup



#### 详细描述



#### 定义：

`FindGroup(i any, raw string) map[string]string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `map[string]string` |   |


 
### re.FindGroupAll



#### 详细描述



#### 定义：

`FindGroupAll(i any, raw string) []map[string]string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `any` |   |
| v2 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `[]map[string]string` |   |


 
### re.FindIndex

提取匹配到的数据索引位置（起止位置）

#### 详细描述



#### 定义：

`FindIndex(origin any, re string) []int`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| index | `[start:int, end:int]` |   |


 
### re.FindSubmatch

正则匹配提取带分组的数据（只匹配一个）

#### 详细描述



#### 定义：

`FindSubmatch(origin any, re string) []string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| results | `[]string` |   |


 
### re.FindSubmatchAll

正则匹配提取带分组的数据（匹配全部）

#### 详细描述



#### 定义：

`FindSubmatchAll(origin any, re string) [][]string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `[][]string` |   |


 
### re.FindSubmatchAllIndex

匹配并提取分组带索引（起止位置）

#### 详细描述



#### 定义：

`FindSubmatchAllIndex(origin any, re string) [][]int`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| indexes | `[][matchStart, matchEnd, group1Start, group1End, ...]` |   |


 
### re.FindSubmatchIndex

只匹配并提取第一组的分组带索引（起止位置）

#### 详细描述



#### 定义：

`FindSubmatchIndex(origin any, re string) []int`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `[]int` |   |


 
### re.Grok

从内容中按照 Grok 规则提取数据

#### 详细描述



#### 定义：

`Grok(string, string) yaklib.GrokResult`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| content | `string` |   |
| grokRule | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| data | `yaklib.GrokResult` |   |


 
### re.Match



#### 详细描述



#### 定义：

`Match(string, any) bool`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| regexpPattern | `string` |  想要匹配的规则 |
| content | `any` |  想要通过正则匹配的数据 |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `bool` |   |


 
### re.MustCompile

编译正则，如果编译失败则 Panic

#### 详细描述



#### 定义：

`MustCompile(string) *regexp.Regexp`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| regexpStr | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `*regexp.Regexp` |   |


 
### re.MustCompilePOSIX

编译正则 POSIX 模式，编译失败则 Panic

#### 详细描述



#### 定义：

`MustCompilePOSIX(string) *regexp.Regexp`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| regexpStr | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `*regexp.Regexp` |   |


 
### re.QuoteMeta

把正则保留字符进行转义

#### 详细描述



#### 定义：

`QuoteMeta(s string) string  doc:QuoteMeta returns a string that escapes all regular expression metacharactersinside the argument text; the returned string is a regular expression matchingthe literal text.`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| v1 | `string` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### re.ReplaceAll

整体批量替换

#### 详细描述



#### 定义：

`ReplaceAll(origin any, re string, newStr any) string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |
| newStr | `any` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 
### re.ReplaceAllWithFunc

正则批量替换数据（使用函数处理匹配结果）

#### 详细描述



#### 定义：

`ReplaceAllWithFunc(origin any, re string, newStr func(string) string) string`


#### 参数

|参数名|参数类型|参数解释|
|:-----------|:---------- |:-----------|
| data | `any` |   |
| regexp | `string` |   |
| replaceFunc | `func (v1: string) return(string) ` |   |





#### 返回值

|返回值(顺序)|返回值类型|返回值解释|
|:-----------|:---------- |:-----------|
| r0 | `string` |   |


 


