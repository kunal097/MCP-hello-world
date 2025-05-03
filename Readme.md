# MCP Hello World
A minimal Model Context Protocol (MCP) server example for practicing MCP server packaging and integration. This project demonstrates how to set up a simple MCP server, define basic resources and tools, and connect it to clients or applications-such as Claude desktop-using standard MCP interfaces.

---


## Getting Started

---
## 🖼️ Screenshot
![App Interface](https://github.com/kunal097/MCP-hello-world/raw/main/assets/sc1.png)

![App Interface](https://github.com/kunal097/MCP-hello-world/raw/main/assets/sc2.png)

![App Interface](https://github.com/kunal097/MCP-hello-world/raw/main/assets/sc3.png)

![App Interface](https://github.com/kunal097/MCP-hello-world/raw/main/assets/sc4.png)

![App Interface](https://github.com/kunal097/MCP-hello-world/raw/main/assets/sc5.png)




### Prerequisites

- Node.js (recommended for running the server)

- MCP-compatible client (e.g., Claude desktop, MCP Inspector)

---

### Installation

1. **Clone the repository**
    ```
    git clone https://github.com/kunal097/MCP-hello-world.git
    cd MCP-hello-world
    ```

2. **Install dependencies**
    ```
    npm i 
    ```

3. **Build Project**
    ```
    npm run build
    ```

---

### Claude Desktop Configuration
To connect this MCP server with Claude desktop, add the following to your Claude settings:


```
{
  "mcpServers": {
    "weather": {
      "command": "node",
      "args": [
        "<path to the code>/weather/build/index.js"
      ]
    }
  }
}
```
`Replace <path to the code> with the actual path to your MCP-hello-world directory.`

### Usage
Once running, the server will respond to MCP-compliant requests. You can use tools like MCP Inspector or compatible clients to interact with the server, test resource fetching, and invoke tools.
