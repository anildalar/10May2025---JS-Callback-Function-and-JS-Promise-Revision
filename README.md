# 10May2025---JS-Callback-Function-and-JS-Promise-Revision
10May2025 - JS Callback Function and JS Promise Revision

1.JavaScript Callbacks Functions (CBFN)
// 1. Function Define (One time)

// 2. Function Call  (Many time)


function



2.JavaScript Promise (Revise)

2.1 JS Promise is JS Class
2.2 JS Promise is built-in Class

JS Promise Chain Structure is Train/Rail

PO.then(cbfn).then(cbfn).then(cbfn).catch(cbfn).finally(cbfn)




PO.then(()=>{}).catch(()=>{}).finally(()=>{})

//1. Class Define

//2. Create class object/Class Instantiation
//let ceo1 = new ClassName();
             //PacalCase
let ceo1 = new Promise((resolve,reject)=>{
      setTimeout(()=>{
        resolve('Hello');
      },5000);
});

//Promise Chain / Train

//Engine.Bogy1.Bogy2.Bogy3..............LastBogy
//PO = Promise Object
//po.then(cbfn).catch(cbfn).finally(cbfn);
ceo1.then((result)=>{
  console.log('then >>>>',result);
}).catch((error)=>{
  console.log('catch >>>>',error);
}).finally(()=>{
  console.log("Finally Block");
});
