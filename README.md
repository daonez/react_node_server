## How to connect react + node (client-server) Basic

---

### [Frontend(client repo)](https://github.com/daonez/react_node_client)

> - [Original Link-FreecodeCamp](https://www.freecodecamp.org/news/create-a-react-frontend-a-node-express-backend-and-connect-them-together-c5798926047c/)
> - [Korean Blog Summary](https://velog.io/@cyongchoi/Node-React-%EC%97%B0%EB%8F%99)

### Code

```JS
1. API Routes Endpoint
const express = require("express")
const router = express.Router()

router.get("/", (req, res, next) => {
  res.send("API is working properly")
})

module.exports = router

2. require/use router, install cors
const cors = require("cors")
const testAPIRouter = require("./routes/testAPI")


app.use("/testAPI", testAPIRouter)
app.use(cors())

```
