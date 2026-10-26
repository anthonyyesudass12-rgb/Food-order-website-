# Food-order-website-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CraveKart | Food Ordering</title>
<style>
:root{--primary:#e7462e;--primary-dark:#c8321e;--ink:#202124;--muted:#6b7280;--bg:#fffaf7;--card:#fff;--line:#eee5df;--green:#16804a;--shadow:0 12px 32px rgba(42,25,15,.08)}
*{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;font-family:Inter,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;background:var(--bg);color:var(--ink)}button,input,select,textarea{font:inherit}button{cursor:pointer}.topbar{position:sticky;top:0;z-index:10;background:rgba(255,255,255,.94);backdrop-filter:blur(14px);border-bottom:1px solid var(--line)}.nav{max-width:1200px;margin:auto;padding:15px 22px;display:flex;align-items:center;gap:24px}.logo{font-size:1.55rem;font-weight:900;letter-spacing:-1px;color:var(--primary);white-space:nowrap}.logo span{color:var(--ink)}.location{font-size:.85rem;color:var(--muted);white-space:nowrap}.location strong{display:block;color:var(--ink);font-size:.95rem}.search{position:relative;flex:1}.search input{width:100%;border:1px solid var(--line);background:#faf8f6;padding:13px 16px 13px 43px;border-radius:13px;outline:none}.search input:focus{border-color:var(--primary);box-shadow:0 0 0 3px #e7462e18}.search .glass{position:absolute;left:15px;top:11px;font-size:1.1rem}.cart-jump{border:0;background:var(--primary);color:white;border-radius:12px;padding:12px 16px;font-weight:800;white-space:nowrap}.cart-jump:hover,.btn-primary:hover{background:var(--primary-dark)}.count{display:inline-grid;place-items:center;background:white;color:var(--primary);min-width:23px;height:23px;border-radius:20px;margin-left:5px;padding:0 5px}.hero{max-width:1200px;margin:24px auto 0;padding:0 22px}.hero-panel{border-radius:26px;overflow:hidden;min-height:280px;display:grid;grid-template-columns:1.15fr .85fr;background:linear-gradient(110deg,#241c19 0%,#3b241e 57%,#8c3522 100%);color:#fff;position:relative}.hero-copy{padding:42px 44px;position:relative;z-index:1}.eyebrow{color:#ffd4a6;text-transform:uppercase;font-size:.78rem;letter-spacing:2px;font-weight:800}.hero h1{font-size:clamp(2.1rem,4vw,3.7rem);line-height:1.05;letter-spacing:-2px;margin:14px 0}.hero h1 em{font-style:normal;color:#ffb15f}.hero p{color:#f2dfd7;max-width:450px;line-height:1.6}.hero-cta{display:inline-block;margin-top:12px;padding:12px 18px;border-radius:12px;background:#fff;color:#30201b;text-decoration:none;font-weight:800}.hero-art{display:grid;place-items:center;font-size:clamp(8rem,18vw,14rem);filter:drop-shadow(0 20px 20px #0005);transform:rotate(-8deg)}.benefits{display:flex;gap:22px;flex-wrap:wrap;margin-top:20px;color:#5e534d;font-size:.88rem}.benefits span{display:flex;align-items:center;gap:7px}.container{max-width:1200px;margin:36px auto;padding:0 22px 60px}.section-heading{display:flex;align-items:end;justify-content:space-between;gap:12px;margin-bottom:18px}.section-heading h2{font-size:1.7rem;letter-spacing:-.8px;margin:0}.section-heading p{color:var(--muted);margin:5px 0 0}.category-row{display:flex;gap:10px;overflow-x:auto;padding:2px 0 15px;margin-bottom:12px}.chip{border:1px solid var(--line);background:white;color:#554c47;border-radius:30px;padding:10px 17px;white-space:nowrap;font-weight:700;transition:.2s}.chip:hover,.chip.active{background:var(--ink);color:white;border-color:var(--ink)}.layout{display:grid;grid-template-columns:minmax(0,1fr) 340px;gap:26px;align-items:start}.food-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px}.food-card{background:var(--card);border:1px solid var(--line);border-radius:18px;overflow:hidden;transition:transform .2s,box-shadow .2s}.food-card:hover{transform:translateY(-4px);box-shadow:var(--shadow)}.food-image{height:160px;position:relative;background:#f4e8df;overflow:hidden}.food-image img{width:100%;height:100%;object-fit:cover;display:block;transition:transform .35s}.food-card:hover .food-image img{transform:scale(1.05)}.badge{position:absolute;top:11px;left:11px;background:#fff;color:var(--green);padding:5px 8px;border-radius:7px;font-size:.72rem;font-weight:900;box-shadow:0 3px 10px #0001}.food-info{padding:14px}.food-title-row{display:flex;justify-content:space-between;gap:8px;align-items:start}.food-title-row h3{margin:0;font-size:1rem}.rating{font-size:.76rem;font-weight:800;background:#e8f6ed;color:#14713d;padding:4px 6px;border-radius:6px;white-space:nowrap}.food-info p{font-size:.82rem;line-height:1.45;color:var(--muted);margin:8px 0 13px;min-height:36px}.food-bottom{display:flex;justify-content:space-between;align-items:center;gap:8px}.price{font-size:1.05rem;font-weight:900}.add-btn{border:1px solid #f1b5a9;color:var(--primary);background:#fff7f4;border-radius:9px;padding:8px 14px;font-weight:900;min-width:76px}.add-btn:hover{background:var(--primary);color:white}.empty-results{grid-column:1/-1;text-align:center;background:white;border:1px dashed var(--line);border-radius:18px;padding:45px 15px;color:var(--muted)}.cart-panel{position:sticky;top:91px;background:#fff;border:1px solid var(--line);border-radius:20px;box-shadow:var(--shadow);overflow:hidden}.cart-header{padding:20px;border-bottom:1px solid var(--line);display:flex;align-items:center;justify-content:space-between}.cart-header h2{margin:0;font-size:1.2rem}.cart-header small{color:var(--muted)}.cart-items{padding:0 18px;max-height:340px;overflow:auto}.cart-empty{text-align:center;padding:30px 10px;color:var(--muted)}.cart-empty .basket{font-size:3rem;display:block;margin-bottom:10px}.cart-item{display:grid;grid-template-columns:52px minmax(0,1fr) auto;gap:10px;padding:15px 0;border-bottom:1px solid #f1ece8;align-items:center}.cart-thumb{width:52px;height:52px;object-fit:cover;border-radius:10px}.cart-item h4{font-size:.86rem;margin:0 0 4px}.cart-item .unit-price{font-size:.78rem;color:var(--muted)}.qty{display:flex;align-items:center;gap:8px;margin-top:7px}.qty button{width:25px;height:25px;border:1px solid var(--line);background:white;border-radius:7px;font-weight:900}.qty button:hover{border-color:var(--primary);color:var(--primary)}.qty span{font-weight:800;font-size:.85rem;min-width:10px;text-align:center}.line-total{font-size:.85rem;font-weight:900;white-space:nowrap}.remove-btn{border:0;background:transparent;color:#9b928c;font-size:.75rem;text-decoration:underline;padding:3px 0}.cart-bottom{padding:18px 20px 20px}.summary-line{display:flex;justify-content:space-between;gap:12px;margin:10px 0;color:#655b55;font-size:.9rem}.summary-line.total{border-top:1px dashed #ded2ca;padding-top:14px;margin-top:14px;color:var(--ink);font-size:1.12rem;font-weight:900}.free-note{font-size:.78rem;color:var(--green);background:#eef9f1;border-radius:8px;padding:9px 10px;margin:12px 0}.checkout-toggle,.btn-primary{width:100%;border:0;border-radius:11px;background:var(--primary);color:#fff;padding:13px 16px;font-weight:900}.checkout-toggle:disabled{background:#d7d1cd;cursor:not-allowed}.checkout{display:none;padding:18px 20px;border-top:1px solid var(--line);background:#fffdfb}.checkout.open{display:block}.checkout h3{margin:0 0 14px}.field{margin-bottom:12px}.field label{display:block;font-size:.8rem;font-weight:800;margin-bottom:5px}.field input,.field textarea,.field select{width:100%;border:1px solid #e6dcd5;border-radius:9px;padding:10px 11px;outline:none;background:white}.field input:focus,.field textarea:focus,.field select:focus{border-color:var(--primary)}.field textarea{resize:vertical;min-height:65px}.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px}.fineprint{font-size:.74rem;color:var(--muted);line-height:1.5;margin:10px 0 0}.toast{position:fixed;left:50%;bottom:24px;transform:translate(-50%,20px);background:#24201e;color:white;padding:12px 18px;border-radius:12px;box-shadow:var(--shadow);opacity:0;pointer-events:none;transition:.25s;z-index:30;max-width:90%;text-align:center}.toast.show{opacity:1;transform:translate(-50%,0)}.success{display:none;padding:28px 22px;text-align:center}.success.show{display:block}.success .check{font-size:3rem}.success h3{margin:10px 0}.success p{color:var(--muted);line-height:1.6}.success button{border:1px solid var(--line);background:white;border-radius:9px;padding:10px 15px;font-weight:800}.footer{background:#251e1b;color:#f8eee8;padding:28px 22px;text-align:center}.footer strong{color:#ffad65}.footer p{color:#c7b8b0;font-size:.85rem;margin:8px 0 0}
@media(max-width:1050px){.layout{grid-template-columns:minmax(0,1fr) 310px}.food-grid{grid-template-columns:repeat(2,minmax(0,1fr))}.nav{gap:14px}.location{display:none}}
@media(max-width:720px){.nav{padding:12px 15px;gap:10px;flex-wrap:wrap}.logo{font-size:1.35rem}.search{order:3;flex-basis:100%}.cart-jump{margin-left:auto;padding:10px 12px}.hero,.container{padding-left:15px;padding-right:15px}.hero{margin-top:15px}.hero-panel{grid-template-columns:1fr;min-height:0}.hero-copy{padding:30px 25px 5px}.hero-art{font-size:7rem;padding:0 0 12px}.hero h1{font-size:2.4rem}.benefits{gap:10px 16px}.container{margin-top:28px}.layout{grid-template-columns:1fr}.cart-panel{position:static;grid-row:1}.cart-items{max-height:280px}.food-grid{grid-template-columns:repeat(2,minmax(0,1fr));gap:12px}.food-image{height:130px}.food-info{padding:11px}.food-info p{font-size:.78rem;min-height:48px}.food-title-row{flex-wrap:wrap}.section-heading h2{font-size:1.45rem}}
@media(max-width:390px){.food-grid{grid-template-columns:1fr}.food-image{height:185px}.food-info p{min-height:0}.form-grid{grid-template-columns:1fr}.hero h1{font-size:2rem}}
</style>
</head>
<body>
<header class="topbar">
  <nav class="nav">
    <div class="logo">Crave<span>Kart.</span></div>
    <div class="location">Delivering to <strong>📍 Your doorstep</strong></div>
    <div class="search"><span class="glass">⌕</span><input id="searchInput" type="search" placeholder="Search biryani, pizza, burger..." aria-label="Search food"></div>
    <button class="cart-jump" id="cartJump">🛒 Cart <span class="count" id="cartCount">0</span></button>
  </nav>
</header>
<section class="hero">
  <div class="hero-panel">
    <div class="hero-copy">
      <div class="eyebrow">Good food. Good mood.</div>
      <h1>Your cravings,<br><em>delivered.</em></h1>
      <p>From comfort-food classics to little treats, discover something delicious for every mood.</p>
      <a class="hero-cta" href="#menu">Explore the menu&nbsp; →</a>
    </div>
    <div class="hero-art" aria-hidden="true">🍔</div>
  </div>
  <div class="benefits"><span>⚡ Freshly prepared</span><span>🛵 Easy ordering</span><span>💛 Made for food lovers</span></div>
</section>
<main class="container" id="menu">
  <div class="section-heading"><div><h2>Explore our menu</h2><p>Find your next favourite bite.</p></div><div id="resultCount" style="font-size:.82rem;color:var(--muted)"></div></div>
  <div class="category-row" id="categories" aria-label="Food categories"></div>
  <div class="layout">
    <section class="food-grid" id="foodGrid" aria-live="polite"></section>
    <aside class="cart-panel" id="cartPanel">
      <div id="cartMain">
        <div class="cart-header"><h2>🛒 Your basket</h2><small id="cartSubtitle">0 items</small></div>
        <div class="cart-items" id="cartItems"></div>
        <div class="cart-bottom">
          <div class="free-note" id="freeNote">Add something tasty to get started!</div>
          <div class="summary-line"><span>Item subtotal</span><strong id="subtotal">₹0</strong></div>
          <div class="summary-line"><span>Delivery fee</span><strong id="delivery">₹0</strong></div>
          <div class="summary-line total"><span>Total</span><strong id="grandTotal">₹0</strong></div>
          <button class="checkout-toggle" id="checkoutToggle" disabled>Proceed to checkout →</button>
        </div>
        <form class="checkout" id="checkoutForm">
          <h3>Delivery details</h3>
          <div class="field"><label for="customerName">Full name *</label><input id="customerName" name="customerName" autocomplete="name" required minlength="2" placeholder="Your name"></div>
          <div class="form-grid">
            <div class="field"><label for="phone">Phone number *</label><input id="phone" name="phone" type="tel" inputmode="numeric" pattern="[0-9]{10}" maxlength="10" required placeholder="10-digit number"></div>
            <div class="field"><label for="payment">Payment method *</label><select id="payment" name="payment" required><option value="">Choose one</option><option>Cash on Delivery</option><option>UPI on Delivery</option></select></div>
          </div>
          <div class="field"><label for="address">Delivery address *</label><textarea id="address" name="address" required minlength="8" placeholder="House / street, area, city, PIN code"></textarea></div>
          <div class="field"><label for="notes">Order notes (optional)</label><input id="notes" name="notes" placeholder="Less spicy, no onions..."></div>
          <button class="btn-primary" type="submit">Place my order · <span id="checkoutTotal">₹0</span></button>
          <p class="fineprint">Demo checkout only. No payment is collected and no restaurant order is sent.</p>
        </form>
      </div>
      <div class="success" id="successPanel">
        <div class="check">✅</div><h3>Order placed!</h3><p id="successMessage"></p><button id="continueShopping">Continue shopping</button>
      </div>
    </aside>
  </div>
</main>
<footer class="footer"><strong>CraveKart.</strong><p>Good food brings people together. Made with ♥ for hungry moments.</p><p>Demo website · Sample menu and prices · No real delivery service</p></footer>
<div class="toast" id="toast" role="status" aria-live="polite"></div>
<script>
"use strict";
const foodItems = [
 {id:1,name:"Classic Cheeseburger",category:"Burgers",price:189,rating:"4.8",tag:"Bestseller",description:"Juicy patty, melted cheese, lettuce & house sauce.",emoji:"🍔",image:"https://images.unsplash.com/photo-1568901346375-23c9450c58cd?auto=format&fit=crop&w=700&q=80"},
 {id:2,name:"Margherita Pizza",category:"Pizza",price:249,rating:"4.7",tag:"Veg favourite",description:"Mozzarella, fresh basil & our signature tomato sauce.",emoji:"🍕",image:"https://images.unsplash.com/photo-1574071318508-1cdbab80d002?auto=format&fit=crop&w=700&q=80"},
 {id:3,name:"Paneer Tikka",category:"Indian",price:219,rating:"4.9",tag:"Popular",description:"Smoky tandoori paneer with peppers and mint chutney.",emoji:"🍢",image:"https://images.unsplash.com/photo-1567188040759-fb8a883dc6d8?auto=format&fit=crop&w=700&q=80"},
 {id:4,name:"Chicken Biryani",category:"Indian",price:279,rating:"4.9",tag:"Chef's pick",description:"Fragrant basmati rice, aromatic spices & tender chicken.",emoji:"🍛",image:"https://images.unsplash.com/photo-1563379091339-03246963d96c?auto=format&fit=crop&w=700&q=80"},
 {id:5,name:"Crispy French Fries",category:"Sides",price:99,rating:"4.6",tag:"Crispy",description:"Golden, lightly salted fries with a satisfying crunch.",emoji:"🍟",image:"https://images.unsplash.com/photo-1573080496219-bb080dd4f877?auto=format&fit=crop&w=700&q=80"},
 {id:6,name:"Garden Fresh Salad",category:"Healthy",price:159,rating:"4.5",tag:"Fresh pick",description:"Crisp greens, cherry tomatoes, cucumber & zesty dressing.",emoji:"🥗",image:"https://images.unsplash.com/photo-1512621776951-a57141f2eefd?auto=format&fit=crop&w=700&q=80"},
 {id:7,name:"Chocolate Brownie",category:"Desserts",price:129,rating:"4.8",tag:"Sweet treat",description:"Rich chocolate brownie with a soft, fudgy centre.",emoji:"🍫",image:"https://images.unsplash.com/photo-1606313564200-e75d5e30476c?auto=format&fit=crop&w=700&q=80"},
 {id:8,name:"Strawberry Milkshake",category:"Drinks",price:139,rating:"4.6",tag:"Chilled",description:"Creamy strawberry shake blended fresh and served cold.",emoji:"🥤",image:"https://images.unsplash.com/photo-1572490122747-3968b75cc699?auto=format&fit=crop&w=700&q=80"},
 {id:9,name:"Double Cheese Burger",category:"Burgers",price:249,rating:"4.7",tag:"Extra cheesy",description:"Two savoury patties layered with cheese and pickles.",emoji:"🍔",image:"https://images.unsplash.com/photo-1553979459-d2229ba7433a?auto=format&fit=crop&w=700&q=80"},
 {id:10,name:"Pepperoni Pizza",category:"Pizza",price:329,rating:"4.8",tag:"Fan favourite",description:"A golden crust topped with cheese and pepperoni.",emoji:"🍕",image:"https://images.unsplash.com/photo-1628840042765-356cda07504e?auto=format&fit=crop&w=700&q=80"},
 {id:11,name:"Masala Dosa",category:"Indian",price:119,rating:"4.7",tag:"South Indian",description:"Crisp dosa with spiced potato, sambar & coconut chutney.",emoji:"🥞",image:"https://images.unsplash.com/photo-1668236543090-82eba5ee5976?auto=format&fit=crop&w=700&q=80"},
 {id:12,name:"Cold Coffee",category:"Drinks",price:119,rating:"4.5",tag:"Cool down",description:"Smooth iced coffee finished with a creamy foam.",emoji:"🧋",image:"https://images.unsplash.com/photo-1461023058943-07fcbe16d735?auto=format&fit=crop&w=700&q=80"}
];
const STORAGE_KEY = "cravekart_cart_v1";
let cart = loadCart();
let activeCategory = "All";
let toastTimer;
const $ = id => document.getElementById(id);
const money = value => "₹" + value.toLocaleString("en-IN");
const categories = ["All", ...new Set(foodItems.map(item => item.category))];

function loadCart(){
 try{
  const saved = JSON.parse(localStorage.getItem(STORAGE_KEY) || "{}");
  const valid = {};
  for(const [id,qty] of Object.entries(saved)){
   if(foodItems.some(item => item.id === Number(id)) && Number.isInteger(qty) && qty > 0 && qty < 100) valid[id] = qty;
  }
  return valid;
 }catch(error){ return {}; }
}
function saveCart(){
 try{localStorage.setItem(STORAGE_KEY, JSON.stringify(cart));}
 catch(error){showToast("Your browser could not save the cart. It may be in private mode.");}
}
function renderCategories(){
 $("categories").innerHTML = categories.map(category =>
  `<button class="chip ${activeCategory===category?"active":""}" data-category="${escapeHTML(category)}">${category==="All"?"🍽️":categoryIcon(category)} ${escapeHTML(category)}</button>`
 ).join("");
}
function categoryIcon(category){
 return ({Burgers:"🍔",Pizza:"🍕",Indian:"🍛",Sides:"🍟",Healthy:"🥗",Desserts:"🍰",Drinks:"🥤"})[category] || "🍴";
}
function renderFood(){
 const query = $("searchInput").value.trim().toLowerCase();
 const filtered = foodItems.filter(item =>
  (activeCategory==="All" || item.category===activeCategory) &&
  (item.name.toLowerCase().includes(query) || item.description.toLowerCase().includes(query) || item.category.toLowerCase().includes(query))
 );
 $("resultCount").textContent = `${filtered.length} ${filtered.length===1?"dish":"dishes"}`;
 if(!filtered.length){
  $("foodGrid").innerHTML = `<div class="empty-results"><div style="font-size:2.5rem">🔎</div><h3>No dishes found</h3><p>Try another search or choose a different category.</p><button class="chip" id="clearSearch">Clear filters</button></div>`;
  return;
 }
 $("foodGrid").innerHTML = filtered.map(item => `
  <article class="food-card">
   <div class="food-image"><img src="${item.image}" alt="${escapeHTML(item.name)}" loading="lazy" onerror="this.onerror=null;this.src='https://placehold.co/700x450/f4e8df/4a342c?text=${encodeURIComponent(item.emoji+" "+item.name)}'"><span class="badge">${escapeHTML(item.tag)}</span></div>
   <div class="food-info">
    <div class="food-title-row"><h3>${escapeHTML(item.name)}</h3><span class="rating">★ ${item.rating}</span></div>
    <p>${escapeHTML(item.description)}</p>
    <div class="food-bottom"><span class="price">${money(item.price)}</span><button class="add-btn" data-add="${item.id}">${cart[item.id] ? "ADD +" : "+ ADD"}</button></div>
   </div>
  </article>`).join("");
}
function getCartItems(){
 return Object.entries(cart).map(([id,qty])=>({item:foodItems.find(item=>item.id===Number(id)),qty})).filter(row=>row.item);
}
function getSubtotal(){return getCartItems().reduce((sum,row)=>sum+row.item.price*row.qty,0);}
function getCount(){return getCartItems().reduce((sum,row)=>sum+row.qty,0);}
function getDelivery(){const subtotal=getSubtotal();return subtotal===0 || subtotal>=499 ? 0 : 30;}
function renderCart(){
 const rows = getCartItems(), count = getCount(), subtotal = getSubtotal(), delivery = getDelivery(), total = subtotal+delivery;
 $("cartCount").textContent=count;
 $("cartSubtitle").textContent=`${count} ${count===1?"item":"items"}`;
 $("cartItems").innerHTML = rows.length ? rows.map(({item,qty})=>`
  <div class="cart-item">
   <img class="cart-thumb" src="${item.image}" alt="" onerror="this.style.visibility='hidden'">
   <div><h4>${escapeHTML(item.name)}</h4><div class="unit-price">${money(item.price)} each</div>
    <div class="qty"><button type="button" data-change="${item.id}" data-delta="-1" aria-label="Decrease ${escapeHTML(item.name)} quantity">−</button><span>${qty}</span><button type="button" data-change="${item.id}" data-delta="1" aria-label="Increase ${escapeHTML(item.name)} quantity">+</button></div>
   </div>
   <div><div class="line-total">${money(item.price*qty)}</div><button type="button" class="remove-btn" data-remove="${item.id}">Remove</button></div>
  </div>`).join("") : `<div class="cart-empty"><span class="basket">🧺</span><strong>Your basket is empty</strong><p>Add a dish you love and it will appear here.</p></div>`;
 $("subtotal").textContent=money(subtotal);
 $("delivery").textContent=delivery===0 ? (subtotal===0 ? money(0) : "FREE") : money(delivery);
 $("grandTotal").textContent=money(total);
 $("checkoutTotal").textContent=money(total);
 $("checkoutToggle").disabled=count===0;
 $("freeNote").textContent=subtotal===0?"Add something tasty to get started!":subtotal>=499?"🎉 You've unlocked free delivery!":`Add ${money(499-subtotal)} more for free delivery.`;
 if(count===0){$("checkoutForm").classList.remove("open");$("checkoutToggle").textContent="Proceed to checkout →";}
}
function addToCart(id){
 cart[id]=(cart[id]||0)+1;saveCart();renderAll();showToast(`${foodItems.find(item=>item.id===id).name} added to your basket.`);
}
function changeQty(id,delta){
 if(!cart[id])return;
 cart[id]+=delta;if(cart[id]<=0)delete cart[id];saveCart();renderAll();
}
function removeItem(id){
 const item=foodItems.find(food=>food.id===id);delete cart[id];saveCart();renderAll();showToast(`${item.name} removed from your basket.`);
}
function renderAll(){renderCategories();renderFood();renderCart();}
function showToast(message){
 const el=$("toast");el.textContent=message;el.classList.add("show");clearTimeout(toastTimer);toastTimer=setTimeout(()=>el.classList.remove("show"),2400);
}
function escapeHTML(value){
 return String(value).replace(/[&<>"']/g,char=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[char]));
}
$("categories").addEventListener("click",event=>{
 const button=event.target.closest("[data-category]");if(!button)return;
 activeCategory=button.dataset.category;renderCategories();renderFood();
});
$("foodGrid").addEventListener("click",event=>{
 const add=event.target.closest("[data-add]");
 if(add){addToCart(Number(add.dataset.add));return;}
 if(event.target.closest("#clearSearch")){$("searchInput").value="";activeCategory="All";renderAll();}
});
$("searchInput").addEventListener("input",renderFood);
$("cartItems").addEventListener("click",event=>{
 const change=event.target.closest("[data-change]"),remove=event.target.closest("[data-remove]");
 if(change)changeQty(Number(change.dataset.change),Number(change.dataset.delta));
 if(remove)removeItem(Number(remove.dataset.remove));
});
$("cartJump").addEventListener("click",()=>{$("cartPanel").scrollIntoView({behavior:"smooth",block:"start"});});
$("checkoutToggle").addEventListener("click",()=>{
 if(getCount()===0)return;
 $("checkoutForm").classList.toggle("open");
 $("checkoutToggle").textContent=$("checkoutForm").classList.contains("open")?"Hide checkout ↑":"Proceed to checkout →";
 if($("checkoutForm").classList.contains("open"))$("customerName").focus({preventScroll:true});
});
$("checkoutForm").addEventListener("submit",event=>{
 event.preventDefault();
 if(getCount()===0){showToast("Your basket is empty.");return;}
 const form=event.currentTarget;
 if(!form.reportValidity())return;
 const name=$("customerName").value.trim(),phone=$("phone").value.trim(),address=$("address").value.trim();
 if(name.length<2 || !/^[0-9]{10}$/.test(phone) || address.length<8){showToast("Please check your details and try again.");return;}
 const orderNumber="CK"+Date.now().toString().slice(-7);
 const total=money(getSubtotal()+getDelivery());
 const summary=getCartItems().map(row=>`${row.qty} × ${row.item.name}`).join(", ");
 $("successMessage").textContent=`Thanks, ${name}! Demo order ${orderNumber} is confirmed for ${total}. Items: ${summary}. Delivery address: ${address}. This is a sample website, so no real restaurant has received the order.`;
 $("cartMain").style.display="none";$("successPanel").classList.add("show");
 cart={};saveCart();renderAll();window.scrollTo({top:$("cartPanel").getBoundingClientRect().top+window.scrollY-100,behavior:"smooth"});
});
$("continueShopping").addEventListener("click",()=>{
 $("successPanel").classList.remove("show");$("cartMain").style.display="block";$("checkoutForm").reset();$("checkoutForm").classList.remove("open");$("checkoutToggle").textContent="Proceed to checkout →";renderAll();$("menu").scrollIntoView({behavior:"smooth"});
});
renderAll();
</script>
</body>
</html>
