<!DOCTYPE html>
<html lang="ne">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>बढई समाज मोरङ | Morang Badhai Samaj</title>
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans+Devanagari:wght@400;600;700;900&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:'Noto Sans Devanagari',sans-serif;background:#FFF8E8;color:#222;overflow-x:hidden}
.topbar{background:#4A0710;color:#fff;padding:8px 14px;display:flex;justify-content:space-between;font-size:13px;flex-wrap:wrap;gap:6px}
.topbar b{color:#F5D67A}
.live-dot{width:9px;height:9px;background:#22C55E;border-radius:50%;display:inline-block;animation:pulse 1.5s infinite}
@keyframes pulse{0%{box-shadow:0 0 0 0 rgba(34,197,94,.6)}70%{box-shadow:0 0 0 8px rgba(34,197,94,0)}100%{box-shadow:0 0 0 0 rgba(34,197,94,0)}}
header{position:sticky;top:0;z-index:100;background:#fff;display:flex;align-items:center;justify-content:space-between;padding:10px 4%;box-shadow:0 4px 20px rgba(0,0,0,.1);gap:10px}
.logo{display:flex;gap:10px;align-items:center}
.logo-circle{width:52px;height:52px;min-width:52px;border-radius:50%;background:#7A0F1F;color:#F5D67A;display:flex;align-items:center;justify-content:center;font-size:28px;font-weight:900;border:3px solid #D4A93C;overflow:hidden}
.logo-circle img{width:100%;height:100%;object-fit:cover}
.logo h1{font-size:20px;color:#7A0F1F;line-height:1.1;white-space:nowrap}
.logo span{font-size:11px;color:#777}
.btn{background:#7A0F1F;color:#fff;padding:11px 18px;border-radius:999px;font-weight:800;text-decoration:none;white-space:nowrap;font-size:14px}
.btn-gold{background:#D4A93C;color:#3A1A00!important}
.hero{background:linear-gradient(135deg,#7A0F1F,#4A0710);color:#fff;padding:36px 5% 42px;display:grid;grid-template-columns:1.1fr .9fr;gap:22px;align-items:center}
.hero h2{font-size:48px;line-height:1.1;margin:12px 0 10px}
.hero h2 span{color:#F5D67A}
.hero-card{background:#fff;color:#222;border-radius:22px;padding:14px;text-align:center}
.hero-card .hero-logo{width:100%;height:280px;border-radius:14px;background:#7A0F1F;color:#fff;display:flex;flex-direction:column;align-items:center;justify-content:center;font-size:60px}
.hero-card .hero-logo small{font-size:18px;color:#F5D67A;margin-top:8px}
.total-live{background:#7A0F1F;color:#fff;padding:16px 18px;border-radius:16px;margin:16px 4% 0;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:10px}
.total-live b{font-size:22px}
.stats{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin:16px 4% 0}
.stat{background:#fff;padding:16px;text-align:center;border-radius:16px;box-shadow:0 8px 25px rgba(0,0,0,.1);border-top:4px solid #D4A93C}
.stat b{font-size:28px;color:#7A0F1F}
.online-badge{display:inline-flex;align-items:center;gap:5px;background:#E8F5E9;color:#157347;padding:4px 10px;border-radius:999px;font-size:12px;font-weight:900;margin-top:4px}
section{padding:42px 4%}
.head{text-align:center;max-width:700px;margin:0 auto 22px}
.head h2{font-size:30px;color:#7A0F1F}
.directory{background:#1A0A0A;color:#fff;border-radius:26px;padding:24px}
.searchbox{display:flex;gap:8px;max-width:600px;margin:16px auto;background:#fff;border-radius:999px;padding:6px}
.searchbox input{flex:1;border:0;outline:0;padding:12px;font-family:inherit;font-size:16px;min-width:0}
.searchbox button{background:#7A0F1F;color:#fff;border:0;padding:12px 18px;border-radius:999px;font-weight:800}
.add-box{background:#fff;color:#222;border-radius:20px;padding:20px;margin-top:20px}
.add-box h3{color:#7A0F1F;margin-bottom:12px}
.add-box input{width:100%;padding:12px;border:1px solid #ddd;border-radius:12px;margin-bottom:10px;font-family:inherit}
.add-box button{background:#7A0F1F;color:#fff;border:0;padding:13px;border-radius:12px;font-weight:900;width:100%;cursor:pointer}
.photo-preview{width:90px;height:90px;border-radius:50%;object-fit:cover;border:3px solid #D4A93C;display:none;margin:0 auto 10px}
.members{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;margin-top:18px}
.member{background:#fff;color:#222;border-radius:18px;padding:16px;text-align:center;position:relative}
.avatar{width:90px;height:90px;border-radius:50%;margin:0 auto;border:3px solid #D4A93C;overflow:hidden;background:#7A0F1F;color:#F5D67A;display:flex;align-items:center;justify-content:center;font-size:36px;font-weight:900}
.avatar img{width:100%;height:100%;object-fit:cover}
.member b{display:block;margin-top:8px}
.member span{font-size:13px;color:#666}
.member a{display:inline-block;margin-top:6px;background:#E8F5E9;color:#1B6B2E;padding:6px 14px;border-radius:999px;font-weight:800;font-size:13px;text-decoration:none}
.member .online-mini{display:inline-flex;align-items:center;gap:4px;font-size:11px;color:#157347;font-weight:800;background:#E8F5E9;padding:3px 8px;border-radius:999px;margin-top:6px}
.member-actions{display:flex;gap:6px;justify-content:center;margin-top:8px}
.member-actions button{border:0;padding:7px 12px;border-radius:999px;font-weight:800;font-size:12px;cursor:pointer}
.btn-edit{background:#FFF2C9;color:#7A0F1F}
.btn-change{background:#E8F0FF;color:#1A4D9E}
.btn-del{background:#FFE8E8;color:#C00}
.del{position:absolute;top:8px;right:8px;background:#ff4444;color:#fff;border:0;width:26px;height:26px;border-radius:50%;cursor:pointer}
.contact{display:grid;grid-template-columns:1fr 1fr;gap:20px;background:linear-gradient(135deg,#7A0F1F,#4A0710);color:#fff;border-radius:26px;padding:24px}
.contact input,.contact textarea{width:100%;padding:12px;border-radius:12px;border:0;margin-bottom:10px;font-family:inherit}
.contact button{background:#D4A93C;border:0;padding:13px;border-radius:12px;font-weight:900;width:100%}
footer{background:#140505;color:#D8C9C9;padding:24px;text-align:center}
.float{position:fixed;right:14px;bottom:14px;background:#25D366;color:#fff;padding:13px 18px;border-radius:999px;font-weight:900;text-decoration:none;z-index:200}
.modal{position:fixed;inset:0;background:rgba(0,0,0,.6);display:none;align-items:center;justify-content:center;z-index:300;padding:16px}
.modal-box{background:#fff;width:100%;max-width:420px;border-radius:20px;padding:20px}
.modal-box input{width:100%;padding:12px;border:1px solid #ddd;border-radius:12px;margin-bottom:10px;font-family:inherit}
.modal-box button{width:100%;padding:12px;border:0;border-radius:12px;font-weight:900;cursor:pointer;margin-bottom:8px}
@media(max-width:900px){.hero{grid-template-columns:1fr;padding:28px 5%}.hero h2{font-size:36px}.stats{grid-template-columns:repeat(2,1fr)}.members{grid-template-columns:repeat(2,1fr)}.contact{grid-template-columns:1fr}}
@media(max-width:520px){.members{grid-template-columns:1fr}.logo h1{font-size:17px}.btn{padding:9px 12px;font-size:13px}}
</style>
</head>
<body>
<div class="topbar"><span>📍 मोरङ | <b>बढई समाज मोरङ</b></span><span><span class="live-dot"></span> <b id="topOnline">1 Online</b> • LIVE</span></div>
<header><div class="logo"><div class="logo-circle"><img src="logo.png" onerror="this.style.display='none'">ॐ</div><div><h1>बढई समाज मोरङ</h1><span>MORANG BADHAI SAMAJ</span></div></div><a class="btn" href="#add">+ सदस्य थप्नुस्</a></header>

<section class="hero" id="home"><div><span style="background:rgba(255,255,255,.15);padding:7px 14px;border-radius:999px;font-weight:700">✨ एकता नै शक्ति हो</span><h2>बढई समाज<br><span>मोरङ</span></h2><p>मोरङभरका सम्पूर्ण बढई / विश्वकर्मा परिवारलाई एउटै डिजिटल निर्देशिकामा जोड्दै।</p><div style="display:flex;gap:10px;margin-top:18px;flex-wrap:wrap"><a class="btn btn-gold" href="#members">🔍 सदस्य खोज्नुस्</a><a class="btn" style="background:#fff;color:#7A0F1F!important" href="#add">📝 नयाँ सदस्य थप्नुस्</a></div></div><div class="hero-card"><div class="hero-logo">ॐ<small>॥ ॐ विश्वकर्मणै नमः ॥</small></div><h3 style="color:#7A0F1F;margin-top:10px">बढई समाज मोरङ</h3><p style="color:#666">सीप, संस्कार र सम्मान — हाम्रो पहिचान</p></div></section>

<div class="total-live"><div style="text-align:left"><span style="opacity:.8;font-size:13px">🟢 LIVE • TOTAL सदस्य</span><br><b><span id="totalCount">1</span> जना सदस्य</b> <span style="background:#22C55E;padding:4px 10px;border-radius:999px;font-size:12px;font-weight:900">● ONLINE</span></div><div style="text-align:right"><span style="opacity:.8;font-size:13px">अहिले Online</span><br><b style="color:#F5D67A"><span id="onlineCount">1</span> जना Online</b></div></div>

<div class="stats"><div class="stat"><b id="count2">1</b><div>जम्मा सदस्य</div><span class="online-badge"><span class="live-dot"></span> <span id="onlineBadge">1 Online</span></span></div><div class="stat"><b>मोरङ</b><div>जिल्ला</div><span class="online-badge"><span class="live-dot"></span> Live</span></div><div class="stat"><b>उर्लाबारी</b><div>मुख्य क्षेत्र</div><span class="online-badge"><span class="live-dot"></span> Live</span></div><div class="stat"><b>100%</b><div>विश्वास</div><span class="online-badge"><span class="live-dot"></span> Active</span></div></div>

<section id="members"><div class="directory"><div class="head" style="color:#fff"><h2 style="color:#fff">डिजिटल निर्देशिका • <span style="color:#22C55E">● LIVE</span></h2><p style="color:#D8C9C9">Total: <b id="totalInDir">1</b> जना | <span style="color:#7CFF9A">● <span id="onlineInDir">1</span> Online</span></p></div><div class="searchbox"><input id="search" placeholder="जस्तै: सन्तोष, उर्लाबारी..." onkeyup="filterMembers()"><button onclick="filterMembers()">खोज्नुस्</button></div><div class="members" id="memberList"></div>
<div class="add-box" id="add"><h3>➕ नयाँ सदस्य थप्नुस् (फोटो सहित)</h3><img id="preview" class="photo-preview"><input type="file" id="photoInput" accept="image/*" onchange="previewPhoto(event)"><p style="font-size:13px;color:#666;text-align:center;margin-bottom:8px">फोटो नहाले नामको अक्षर देखिन्छ, पछि फेर्न मिल्छ</p><input id="fName" placeholder="पूरा नाम *"><input id="fPhone" placeholder="मोबाइल नम्बर *"><input id="fPlace" placeholder="ठेगाना * जस्तै: उर्लाबारी - 7"><input id="fWork" placeholder="काम / व्यवसाय"><button onclick="addMember()">सदस्य थप्नुस् ✅</button><p id="addMsg" style="text-align:center;font-weight:800;color:green;margin-top:8px"></p></div></div></section>

<section id="contact"><div class="contact"><div><h2>सम्पर्क 🙏</h2><p>📞 <b>9815996894 - सन्तोष शर्मा</b><br>📍 <b>उर्लाबारी - 7, मोरङ</b></p><p style="margin-top:10px"><span class="live-dot"></span> अहिले <b id="contactOnline">1</b> जना Online छन्</p></div><form onsubmit="event.preventDefault();document.getElementById('cmsg').innerText='✅ धन्यवाद!'"><input placeholder="पूरा नाम"><input placeholder="मोबाइल नम्बर"><textarea rows="3" placeholder="सन्देश..."></textarea><button>पठाउनुस् →</button><p id="cmsg" style="text-align:center;font-weight:800;margin-top:8px"></p></form></div></section>

<footer><b style="color:#fff">बढई समाज मोरङ</b><br>© 2026 • एकता • सीप • संस्कार • विकास</footer>
<a class="float" href="https://wa.me/9779815996894">💬 WhatsApp</a>

<!-- EDIT / CHANGE PHOTO MODAL -->
<div class="modal" id="editModal"><div class="modal-box"><h3 style="color:#7A0F1F;margin-bottom:12px">✏️ सदस्य Edit / फोटो फेर्नुस्</h3><img id="editPreview" style="width:90px;height:90px;border-radius:50%;object-fit:cover;display:block;margin:0 auto 10px;background:#eee"><input type="file" id="editPhoto" accept="image/*" onchange="previewEditPhoto(event)"><input id="eName" placeholder="पूरा नाम"><input id="ePhone" placeholder="मोबाइल नम्बर"><input id="ePlace" placeholder="ठेगाना"><input id="eWork" placeholder="काम / व्यवसाय"><button style="background:#7A0F1F;color:#fff" onclick="saveEdit()">Save गर्नुस् ✅</button><button style="background:#eee" onclick="closeModal()">Cancel</button></div></div>
<input type="file" id="hiddenPhoto" accept="image/*" style="display:none" onchange="changePhotoFile(event)">

<script>
let defaultMembers=[{name:"सन्तोष शर्मा",phone:"9815996894",place:"उर्लाबारी - 7",work:"बढई समाज मोरङ - सदस्य",img:""}];
let saved=JSON.parse(localStorage.getItem('morang_members_v2')||'[]');
// पुरानो auto photo भएको data भए सफा गर्ने
saved=saved.map(m=>({...m, img: (m.img||'').includes('pravatar')?'':m.img}));
let members=[...defaultMembers,...saved];
let tempPhoto="", editIndex=-1, editPhotoTemp="", changePhotoIndex=-1;
function getInitial(name){return (name||'?').trim().charAt(0)}
function avatarHTML(m){return m.img?`<div class="avatar"><img src="${m.img}"></div>`:`<div class="avatar">${getInitial(m.name)}</div>`}
function updateLiveCounts(){
  let total=members.length;let online=total;
  document.getElementById('totalCount').innerText=total;
  document.getElementById('count2').innerText=total;
  document.getElementById('totalInDir').innerText=total;
  document.getElementById('onlineCount').innerText=online;
  document.getElementById('onlineBadge').innerText=online+" Online";
  document.getElementById('onlineInDir').innerText=online;
  document.getElementById('topOnline').innerText=online+" Online";
  document.getElementById('contactOnline').innerText=online;
}
function previewPhoto(e){let f=e.target.files[0];if(!f)return;let r=new FileReader();r.onload=function(ev){tempPhoto=ev.target.result;let p=document.getElementById('preview');p.src=tempPhoto;p.style.display='block'};r.readAsDataURL(f)}
function render(list){
  document.getElementById('memberList').innerHTML=list.map((m,i)=>{
    let realIdx=members.indexOf(m);
    return `<div class="member">${realIdx>0?`<button class="del" onclick="deleteMember(${realIdx})">✕</button>`:''}${avatarHTML(m)}<b>${m.name}</b><span>${m.place} • ${m.work}</span><br><span class="online-mini"><span class="live-dot" style="width:7px;height:7px"></span> Online</span><br><a href="tel:${m.phone}">📞 ${m.phone}</a><br><a href="https://wa.me/977${m.phone}" style="background:#25D366;color:#fff">💬 WhatsApp</a><div class="member-actions"><button class="btn-change" onclick="openChangePhoto(${realIdx})">📷 फोटो फेर्नुस्</button><button class="btn-edit" onclick="openEdit(${realIdx})">✏️ Edit</button></div>${realIdx>0?`<div><button class="btn-del" style="border:0;padding:6px 12px;border-radius:999px;font-weight:800;font-size:12px;cursor:pointer;margin-top:6px" onclick="deleteMember(${realIdx})">🗑️ Delete</button></div>`:''}</div>`
  }).join('');
  updateLiveCounts();
}
function filterMembers(){let q=document.getElementById('search').value.toLowerCase();render(members.filter(m=>(m.name+m.place+m.work+m.phone).toLowerCase().includes(q)))}
function addMember(){
  let n=document.getElementById('fName').value.trim(),p=document.getElementById('fPhone').value.trim(),pl=document.getElementById('fPlace').value.trim(),w=document.getElementById('fWork').value.trim()||'बढई / विश्वकर्मा';
  if(!n||!p||!pl){alert('कृपया नाम, नम्बर र ठेगाना भर्नुस्');return}
  let nm={name:n,phone:p,place:pl,work:w,img:tempPhoto||''};
  saved.push(nm);localStorage.setItem('morang_members_v2',JSON.stringify(saved));members=[...defaultMembers,...saved];render(members);
  document.getElementById('addMsg').innerText='✅ '+n+' थपियो! अब Total '+members.length+' जना भयो';
  ['fName','fPhone','fPlace','fWork'].forEach(id=>document.getElementById(id).value='');tempPhoto='';document.getElementById('preview').style.display='none';document.getElementById('photoInput').value='';
}
function deleteMember(idx){if(!confirm('हटाउने हो?'))return;let ri=idx-1;saved.splice(ri,1);localStorage.setItem('morang_members_v2',JSON.stringify(saved));members=[...defaultMembers,...saved];render(members)}
function openChangePhoto(idx){changePhotoIndex=idx;document.getElementById('hiddenPhoto').click()}
function changePhotoFile(e){let f=e.target.files[0];if(!f||changePhotoIndex<0)return;let r=new FileReader();r.onload=function(ev){let url=ev.target.result;if(changePhotoIndex===0){defaultMembers[0].img=url}else{saved[changePhotoIndex-1].img=url;localStorage.setItem('morang_members_v2',JSON.stringify(saved))}members=[...defaultMembers,...saved];render(members);alert('✅ फोटो फेरियो!')};r.readAsDataURL(f);e.target.value=''}
function openEdit(idx){editIndex=idx;editPhotoTemp=members[idx].img||'';document.getElementById('eName').value=members[idx].name;document.getElementById('ePhone').value=members[idx].phone;document.getElementById('ePlace').value=members[idx].place;document.getElementById('eWork').value=members[idx].work;let p=document.getElementById('editPreview');if(editPhotoTemp){p.src=editPhotoTemp}else{p.src='';p.style.background='#eee'}document.getElementById('editModal').style.display='flex'}
function previewEditPhoto(e){let f=e.target.files[0];if(!f)return;let r=new FileReader();r.onload=function(ev){editPhotoTemp=ev.target.result;document.getElementById('editPreview').src=editPhotoTemp};r.readAsDataURL(f)}
function saveEdit(){
  let n=document.getElementById('eName').value.trim(),p=document.getElementById('ePhone').value.trim(),pl=document.getElementById('ePlace').value.trim(),w=document.getElementById('eWork').value.trim();
  if(!n||!p||!pl){alert('नाम, नम्बर, ठेगाना चाहिन्छ');return}
  let updated={name:n,phone:p,place:pl,work:w,img:editPhotoTemp};
  if(editIndex===0){defaultMembers[0]=updated}else{saved[editIndex-1]=updated;localStorage.setItem('morang_members_v2',JSON.stringify(saved))}
  members=[...defaultMembers,...saved];render(members);closeModal();alert('✅ Save भयो!');
}
function closeModal(){document.getElementById('editModal').style.display='none'}
render(members);
</script>
</body>
</html>
