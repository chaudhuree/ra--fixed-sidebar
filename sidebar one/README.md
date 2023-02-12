## notes

- App js a MainPage ta k BrowerRouter er moddhe rakhte hobe

```
      <BrowserRouter>
        <MainPage />
      </BrowserRouter>
```

- MainPage ta akhn tahole render hobe react app open korlei

- MainPage a akhn 2 ta part. akta navbar r akta section jetay sidebar and navpage

- akhn 2nd part tay grid kore col-12 k 2 ta col a devide kore aktay col-3 and onnotay col-9 dea dilei tara pasha pashi thakbe.
- Sidebar a data folder theke routing gulo dea Navlink make korbo

```
       SidebarData.map((item, index)=>{
       return(
           <div key={index}>
               <NavLink to={item.path}
               className={({ isActive }) =>
               isActive ? activeLink: normalLink}

                 >
               <span>{item.icon}</span>
               <span>{item.title}</span>
               </NavLink>

           </div>
       )
     })
```

- And navpage a routing kore different page render korlei done.

```
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
        <Route path="/contact" element={<Contact />} />
      </Routes>
```
