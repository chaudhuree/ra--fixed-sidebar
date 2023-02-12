## Note:

<a href="https://ibb.co/K0mKHKF"><img src="https://i.ibb.co/PmtD8Dw/nav-Expand.png" alt="nav-Expand" border="0"></a>

<a href="https://ibb.co/dtV0TS1"><img src="https://i.ibb.co/XDKZQ9N/nav-Collapse.png" alt="nav-Collapse" border="0"></a>

- sidebare name a akta component create korete hobe
- App.js a browser router er moddhe sidebar component er moddhe sob routing page gulo wrap kore dite hobe.

```
    <BrowserRouter>
      <Sidebar>
        <Routes>
          <Route path="/" element={<Dashboard />} />
          <Route path="/dashboard" element={<Dashboard />} />
          <Route path="/about" element={<About />} />
          <Route path="/comment" element={<Comment />} />
          <Route path="/analytics" element={<Analytics />} />
          <Route path="/product" element={<Product />} />
          <Route path="/productList" element={<ProductList />} />
        </Routes>
      </Sidebar>
    </BrowserRouter>
```

- sidebar component a duita part thakbe akta te sidebar thakbe r aktay children thakbe mane routing page gulo thakbe
- then css dea display flex kore dilei pasha pashi thakbe
