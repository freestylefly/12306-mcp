<p align="center"><img src= "https://cdn.canghecode.com/blog/12306-mcp-logo.png" alt="MaxKB" width="300" /></p>
<h3 align="center">一个基于MCP的12306购票搜索服务器</h3>
<p align="center">
  <a href="https://opensource.org/license/MIT"><img src="https://img.shields.io/github/license/freestylefly/12306-mcp?color=rgb(25%2C%20121%2C%20255)" alt="The MIT License"></a>
  <a href=""><img src="https://img.shields.io/github/forks/freestylefly/12306-mcp?color=green" alt="Forks"></a>
  <a href="https://canghecode.com/"><img src="https://img.shields.io/badge/介绍-%E5%AE%98%E7%BD%91-green" alt="Official"></a>
  <a href="https://mp.weixin.qq.com/s/j6c_GjV7nqNTsCpRXMw5tw"><img src="https://img.shields.io/github/stars/freestylefly/12306-mcp?style=flat-square&color=rgb(25%2C%20121%2C%20255)" alt="Stars"></a>    
  <a href="https://mp.weixin.qq.com/s/j6c_GjV7nqNTsCpRXMw5tw"><img src="https://img.shields.io/badge/12306 MCP-教程-blue" alt="Experience"></a>  
</p>

<hr/>

A 12306 ticket search server based on the Model Context Protocol (MCP). The server provides a simple API interface that allows users to search for 12306 tickets.

基于 Model Context Protocol (MCP) 的12306购票搜索服务器。提供了简单的API接口，允许大模型利用接口搜索12306购票信息。

<a href="https://glama.ai/mcp/servers/@freestylefly/12306-mcp">
  <img width="380" height="200" src="https://glama.ai/mcp/servers/@freestylefly/12306-mcp/badge" alt="12306-MCP MCP server" />
</a>

## <div align="center">🔥应用</div>

1、在 Cursor 中使用

可以智能选票还能生成途径站点可视化地图！

教程：[Cursor + 12306 MCP，实现AI智能选票还能生成精美网站](https://mp.weixin.qq.com/s/j6c_GjV7nqNTsCpRXMw5tw)

![](https://cdn.canghecode.com/blog/20250526133600.png)

在yb.html中可直接用浏览器打开

![](https://cdn.canghecode.com/blog/12306.gif)




2、用阿里云百炼做智能体

教程：[阿里百炼+12306 MCP，打造AI智能选票智能体，超酷的！](https://mp.weixin.qq.com/s/saCkwby6qhfpkuiUvRrlrw)

![](https://cdn.canghecode.com/blog/20250528113134.png)

>我在后天想从西安出发去往郑州，请推荐出合理的车票，并推荐三天后返程的车票，

![](https://cdn.canghecode.com/blog/20250528123911.png)

还能对比各个列车票价，做个图表，更直观了。

![](https://cdn.canghecode.com/blog/20250528113238.png)

同样能让他生成列车停靠站点地图：

![](https://cdn.canghecode.com/blog/20250526133600.png)

还能生成途径站点的旅行攻略。这里我的逻辑是先让他去网上搜，搜不到就调用文生图模型，由 AI 生成图片。

![](https://cdn.canghecode.com/blog/20250528122134.png)

阿里自带的这个生图 MCP 感觉能力还是挺强的。

![](https://cdn.canghecode.com/blog/20250528122212.png)

感觉跟真的也差不多啊，哈哈哈。

![](https://cdn.canghecode.com/blog/20250528122245.png)

说实话，在火车上看着自己坐的这一趟列车途径的城市，看着这些景点，心中难免有一丝丝的冲动。

![](https://cdn.canghecode.com/blog/20250528122345.png)




## <div align="center">🚩Features</div>
<div align="center"> 

| 功能描述                         | 状态     |
|------------------------------|--------|
| 查询12306购票信息              | ✅ 已完成  |
| 过滤列车信息                   | ✅ 已完成  |
| 过站查询                      | ✅ 已完成 |
| 中转查询                      | ✅ 已完成 |
| 其余接口，欢迎提feature         | 🚧 计划内 |

</div>
<div align="center"> 
  <img src="https://cdn.canghecode.com/blog/20250526112720.png" width=800px/>
</div>
<div align="center"> 
  <img src="https://cdn.canghecode.com/blog/20250526113041.png" width=800px/>
</div>

## <div align="center">⚙️Installation</div>

~~~bash
git clone https://github.com/freestylefly/12306-mcp.git
npm i
~~~


## <div align="center">▶️Quick Start</div>

### CLI
~~~bash
npm run build
node ./build/index.js
~~~

### MCP sever configuration

~~~json
{
    "mcpServers": {
        "12306-mcp": {
            "command": "npx",
            "args": [
                "-y",
                "12306-mcp"
            ]
        }
    }
}
~~~




## <div align="center">👉️Reference</div>
- [modelcontextprotocol/modelcontextprotocol](https://github.com/modelcontextprotocol/modelcontextprotocol)
- [modelcontextprotocol/typescript-sdk](https://github.com/modelcontextprotocol/typescript-sdk)

## <div align="center">💭Murmurs</div>
本项目原自[12306-MCP](https://github.com/Joooook/12306-mcp) ，感谢作者，本项目仅用于学习，欢迎催更。

## <div align="center">👉️友情链接</div>


- [mcp-server-weread](https://github.com/freestylefly/mcp-server-weread) ：🚀基于 Model Context Protocol (MCP) 的12306购票搜索服务器。提供了简单的API接口，允许大模型利用接口搜索12306购票信息。
- [12306-MCP](https://github.com/Joooook/12306-mcp) ：🚀一个为微信读书提供MCP（Model Context Protocol）服务的工具，支持将微信读书的书籍、笔记和划线数据提供给支持MCP的大语言模型客户端，如Claude Desktop。
- [CodeCanvas](https://github.com/freestylefly/CodeCanvas) ：📚本代码仓库是作者苍何多年从事一线互联网Java开发的学习历程技术汇总，旨在为大家提供一个清晰详细的学习教程，侧重点更倾向编写Java核心内容。💪🏻
- [PmHub](https://github.com/laigeoffer/pmhub) ：🔥PmHub 是一套基于 SpringCloud & LLM 的微服务智能项目管理系统，这个项目旨在帮助小伙伴们快速掌握微服务/分布式项目的架构设计和开发流程，如果想在校招或者社招中拿到一个满意的 offer，PmHub 将是一个非常 nice 的选择。

## star 趋势图

[![Star History Chart](https://api.star-history.com/svg?repos=freestylefly/mcp-server-weread&type=Date)](https://star-history.com/#freestylefly/mcp-server-weread&Date)

## 公众号

微信搜 **苍何** 或扫描下方二维码关注苍何的原创公众号，回复 **AI** 即可和 5000+ 好友一同探讨AI，一同学习MCP。

![苍何微信公众号](https://cdn.tobebetterjavaer.com/stutymore/%E6%89%AB%E7%A0%81_%E6%90%9C%E7%B4%A2%E8%81%94%E5%90%88%E4%BC%A0%E6%92%AD%E6%A0%B7%E5%BC%8F-%E6%A0%87%E5%87%86%E8%89%B2%E7%89%88.png)


## 开源协议

[MIT License (MIT)](https://opensource.org/licenses/MIT)<hr/>
The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

Copyright (c) 2025-2026 12306-MCP