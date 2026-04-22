<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no">
<title>AssisTrip - AI Travel Concierge</title>
<style>
:root{
  --pri:#0A84FF;--pri-dk:#0066CC;--bg:#F2F2F7;--card:#FFF;--tx:#1C1C1E;--txs:#8E8E93;
  --red:#FF3B30;--red-bg:#FFEBEA;--grn:#34C759;--grn-bg:#E5F9EB;--org:#FF9500;--org-bg:#FFF4E5;
  --ic:linear-gradient(135deg,#2E3192,#1BFFFF);
  --jp:#C8102E;
  --r-lg:20px;--r-md:16px;--r-sm:12px;
  --s-sm:0 2px 8px rgba(0,0,0,.04);--s-md:0 4px 16px rgba(0,0,0,.08);--s-lg:0 12px 32px rgba(0,0,0,.15);
}
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
body{font-family:-apple-system,BlinkMacSystemFont,"Helvetica Neue","Segoe UI","Hiragino Kaku Gothic ProN",sans-serif;background:#E5E5EA;color:var(--tx);line-height:1.5}
body.no-header .g-hdr,body.no-header .fab{display:none}
.app{max-width:430px;margin:0 auto;background:var(--bg);min-height:100vh;position:relative;overflow-x:hidden;box-shadow:var(--s-lg)}
.g-hdr{position:sticky;top:0;z-index:50;background:var(--bg);display:flex;align-items:center;padding:12px 16px;border-bottom:1px solid #E5E5EA;gap:10px}
.g-hdr .ham{width:36px;height:36px;border:none;background:none;cursor:pointer;display:flex;flex-direction:column;justify-content:center;gap:5px;padding:6px}
.g-hdr .ham span{display:block;height:2px;background:var(--tx);border-radius:1px;transition:.3s}
.g-hdr .logo{font-size:20px;font-weight:800;letter-spacing:-.5px;color:var(--pri);cursor:pointer;font-style:italic}
.g-hdr .logo sub{font-size:11px;font-weight:600;color:var(--txs);font-style:normal;vertical-align:baseline;margin-left:2px}
.admin-badge{display:inline-flex;align-items:center;gap:4px;background:linear-gradient(135deg,#FF6B6B,#EE5A24);color:#fff;font-size:10px;font-weight:700;padding:3px 8px;border-radius:10px;letter-spacing:.5px;margin-left:auto;text-transform:uppercase;box-shadow:0 2px 6px rgba(238,90,36,.3)}
.admin-tabs{display:flex;background:var(--card);border-bottom:1px solid #E5E5EA;padding:0 16px;gap:0}
.admin-tabs .atab{flex:1;padding:10px 8px;border:none;background:transparent;font-size:13px;font-weight:700;color:var(--txs);cursor:pointer;border-bottom:2px solid transparent;transition:.2s;text-align:center}
.admin-tabs .atab.act{color:var(--pri);border-bottom-color:var(--pri)}
.admin-tabs .atab:active{background:#F9F9F9}
.admin-section{background:var(--card);border-radius:var(--r-md);padding:16px;box-shadow:var(--s-sm);margin-bottom:16px}
.admin-section h3{font-size:15px;font-weight:700;margin-bottom:12px;display:flex;align-items:center;gap:8px}
.admin-section .adesc{font-size:12px;color:var(--txs);line-height:1.5;margin-bottom:12px}
.admin-field{margin-bottom:14px}
.admin-field label{display:block;font-size:13px;font-weight:600;color:var(--tx);margin-bottom:6px}
.admin-field .af-input-wrap{display:flex;align-items:center;gap:8px}
.admin-field .af-input-wrap input,.admin-field .af-input-wrap select,.admin-field .af-input-wrap textarea{flex:1;background:#F2F2F7;border:1px solid #E5E5EA;padding:12px 14px;border-radius:var(--r-sm);font-size:14px;outline:none;color:var(--tx);font-weight:600;font-family:inherit}
.admin-field .af-input-wrap textarea{min-height:120px;resize:vertical;line-height:1.5}
.admin-field .af-input-wrap input:focus,.admin-field .af-input-wrap select:focus,.admin-field .af-input-wrap textarea:focus{border-color:var(--pri);box-shadow:0 0 0 3px rgba(10,132,255,.12)}
.admin-field .af-input-wrap input::placeholder,.admin-field .af-input-wrap textarea::placeholder{color:var(--txs);font-weight:400}
.toggle-vis{width:36px;height:36px;border-radius:8px;border:1px solid #E5E5EA;background:var(--card);cursor:pointer;display:flex;align-items:center;justify-content:center;color:var(--txs);flex-shrink:0;font-size:16px;transition:.15s}
.toggle-vis:active{background:#F2F2F7}
.api-help-card{background:#F9F9FB;border:1px solid #EAEAEE;border-radius:var(--r-sm);padding:12px 14px;margin-bottom:10px}
.api-help-card .ahc-title{font-size:13px;font-weight:700;margin-bottom:4px;display:flex;align-items:center;gap:6px}
.api-help-card a{color:var(--pri);font-size:12px;font-weight:600;text-decoration:none;word-break:break-all;display:inline-flex;align-items:center;gap:4px;line-height:1.4}
.api-help-card a:hover{text-decoration:underline}
.api-help-card .ahc-note{font-size:11px;color:var(--txs);margin-top:4px;line-height:1.4}
.login-admin-toggle{text-align:center;margin-top:16px}
.login-admin-toggle button{background:none;border:none;color:var(--pri);font-size:13px;font-weight:600;cursor:pointer;padding:8px 16px;border-radius:8px;transition:.15s}
.login-admin-toggle button:active{background:#F0F8FF}
.login-admin-fields{max-height:0;overflow:hidden;transition:max-height .3s ease;opacity:0}
.login-admin-fields.open{max-height:200px;opacity:1;transition:max-height .3s ease,opacity .3s ease}
.menu-overlay{position:fixed;inset:0;background:rgba(0,0,0,.45);z-index:150;opacity:0;pointer-events:none;transition:opacity .3s}
.menu-overlay.open{opacity:1;pointer-events:auto}
.side-menu{position:fixed;top:0;left:0;bottom:0;width:280px;max-width:80vw;background:var(--card);z-index:160;transform:translateX(-100%);transition:transform .3s cubic-bezier(.4,0,.2,1);display:flex;flex-direction:column;box-shadow:var(--s-lg)}
.side-menu.open{transform:translateX(0)}
.side-menu header{padding:24px 20px 16px;border-bottom:1px solid #E5E5EA}
.side-menu header .logo{font-size:22px;font-weight:800;color:var(--pri);font-style:italic}
.side-menu nav{flex:1;overflow-y:auto;padding:8px 0}
.side-menu nav a{display:flex;align-items:center;gap:14px;padding:14px 20px;font-size:15px;font-weight:600;color:var(--tx);text-decoration:none;transition:background .15s;cursor:pointer}
.side-menu nav a:active,.side-menu nav a.cur{background:#F0F8FF;color:var(--pri)}
.side-menu nav a svg{width:22px;height:22px;color:var(--txs);flex-shrink:0}
.side-menu nav a.cur svg{color:var(--pri)}
.sh{display:flex;align-items:center;padding:12px 20px;gap:12px}
.sh h2{font-size:17px;font-weight:700;flex:1}
.sh .back{width:32px;height:32px;border-radius:16px;background:#E5E5EA;border:none;display:flex;align-items:center;justify-content:center;cursor:pointer;color:var(--tx);flex-shrink:0}
.sh .back:active{transform:scale(.92)}
.view{display:none;width:100%;min-height:calc(100vh - 52px);padding-bottom:100px;animation:fadeV .25s ease}
.view.active{display:block}
@keyframes fadeV{from{opacity:0;transform:translateX(8px)}to{opacity:1;transform:translateX(0)}}
.sec{padding:0 20px 24px}
.sec-t{font-size:16px;font-weight:700;margin-bottom:12px;display:flex;justify-content:space-between;align-items:center}
.sec-t small{font-size:11px;color:var(--txs);font-weight:500}
.mt3{margin-top:12px}.mt4{margin-top:16px}.mb2{margin-bottom:8px}.mb3{margin-bottom:12px}.mb4{margin-bottom:16px}
.ts{font-size:13px}.txs{font-size:11px}.fw7{font-weight:700}.fsub{color:var(--txs)}
.fx{display:flex}.fxc{display:flex;flex-direction:column}.aic{align-items:center}.jcsb{justify-content:space-between}
.g2{gap:8px}.g3{gap:12px}.g4{gap:16px}
.w100{width:100%}.tac{text-align:center}.tar{text-align:right}
.card{background:var(--card);border-radius:var(--r-md);padding:16px;box-shadow:var(--s-sm);margin-bottom:16px}
.card.flat{box-shadow:none;border:1px solid #E5E5EA}
.card.grad{background:var(--ic);color:#fff;border:none}
.pay-card{background:#1A1A1A;border-radius:var(--r-lg);padding:24px;color:#fff;position:relative;overflow:hidden;box-shadow:var(--s-md);margin-bottom:24px;cursor:pointer;transition:transform .2s}
.pay-card:active{transform:scale(.98)}
.pay-card::before{content:'';position:absolute;inset:0;background:var(--ic);opacity:.15}
.pay-card>*{position:relative;z-index:1}
.pay-label{font-size:13px;opacity:.8;margin-bottom:4px}
.pay-bal{font-size:36px;font-weight:800;letter-spacing:-1px;margin-bottom:24px}
.pay-status{background:rgba(255,255,255,.2);padding:4px 10px;border-radius:12px;font-size:11px;font-weight:600;display:flex;align-items:center;gap:4px;backdrop-filter:blur(4px)}
.pay-status::before{content:'';width:6px;height:6px;border-radius:50%;background:var(--grn)}
.btn{border:none;border-radius:var(--r-sm);padding:14px;font-size:15px;font-weight:600;cursor:pointer;text-align:center;transition:opacity .2s,transform .1s;display:block;width:100%}
.btn:active{transform:scale(.98)}
.bp{background:var(--pri);color:#fff}
.bs{background:rgba(255,255,255,.15);color:#fff;backdrop-filter:blur(8px)}
.bo{border:2px solid var(--pri);color:var(--pri);background:transparent}
.btn-row{display:flex;gap:12px}
.btn-row .btn{flex:1}
.ml{background:var(--card);border-radius:var(--r-md);overflow:hidden;box-shadow:var(--s-sm);margin-bottom:16px}
.mi{display:flex;align-items:center;justify-content:space-between;padding:16px;border-bottom:1px solid #F2F2F7;cursor:pointer;transition:background .15s}
.mi:active{background:#F9F9F9}
.mi:last-child{border-bottom:none}
.mi.act{background:#F0F8FF}
.mi-tx{font-size:15px;font-weight:600;display:flex;align-items:center;gap:12px}
.mi-tx svg{color:var(--txs);width:22px;height:22px}
.mi.act .mi-tx svg{color:var(--pri)}
.mi-sub{font-size:12px;color:var(--txs);margin-top:4px;padding-left:34px}
.chev{color:#C7C7CC;width:20px;height:20px;flex-shrink:0}
.radio{width:22px;height:22px;border-radius:11px;border:2px solid #C7C7CC;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.mi.act .radio{border-color:var(--pri)}
.mi.act .radio::after{content:'';width:10px;height:10px;background:var(--pri);border-radius:5px}
.sel-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px}
.sel-grid.g3c{grid-template-columns:1fr 1fr 1fr}
.sel-grid.g4c{grid-template-columns:1fr 1fr 1fr 1fr}
.sel-btn{border:2px solid #E5E5EA;background:var(--card);padding:12px;border-radius:var(--r-sm);font-size:14px;font-weight:700;color:var(--tx);cursor:pointer;transition:.2s;text-align:center}
.sel-btn.act{border-color:var(--pri);background:#F0F8FF;color:var(--pri)}
.sel-btn small{display:block;font-size:11px;font-weight:500;color:var(--txs);margin-top:4px}
.sel-btn.act small{color:var(--pri);opacity:.8}
.qgrid{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.qbtn{background:var(--card);border-radius:var(--r-md);padding:16px 12px;text-align:center;border:none;box-shadow:var(--s-sm);cursor:pointer;transition:background .2s;display:flex;flex-direction:column;align-items:center;gap:10px}
.qbtn:active{background:#F9F9F9;transform:scale(.98)}
.icn-c{width:44px;height:44px;border-radius:22px;background:#F0F8FF;display:flex;align-items:center;justify-content:center;color:var(--pri)}
.qbtn span{font-size:13px;font-weight:600;line-height:1.2}
.badge{padding:4px 8px;border-radius:8px;font-size:11px;font-weight:700;display:inline-flex;align-items:center;gap:4px}
.b-grn{color:var(--grn);background:var(--grn-bg);border:1px solid #BDE0FE}
.b-org{color:var(--org);background:var(--org-bg);border:1px solid #FFE0B2}
.b-red{color:var(--red);background:var(--red-bg);border:1px solid #FFC6C4}
.b-blu{color:var(--pri-dk);background:#F0F8FF;border:1px solid #BDE0FE}
.gi{display:flex;align-items:flex-start;gap:12px;padding:12px 0;border-bottom:1px dashed #E5E5EA}
.gi:last-child{border-bottom:none;padding-bottom:0}
.gi-icon{background:#F0F8FF;color:var(--pri);padding:8px;border-radius:12px;flex-shrink:0}
.gi h4{font-size:14px;font-weight:700;margin-bottom:4px}
.gi p{font-size:12px;color:var(--txs);line-height:1.4}
.sbox{background:var(--card);border-radius:var(--r-md);padding:16px;box-shadow:var(--s-sm);margin-bottom:16px}
.irow{display:flex;align-items:center;gap:12px;margin-bottom:12px}
.irow:last-child{margin-bottom:0}
.irow .ii{color:var(--pri);width:24px;text-align:center;flex-shrink:0}
.ifield{flex:1;background:#F2F2F7;border:none;padding:14px 16px;border-radius:var(--r-sm);font-size:15px;outline:none;color:var(--tx);font-weight:600;min-width:0}
.ifield::placeholder{color:var(--txs);font-weight:400}
.divider{height:1px;background:#E5E5EA;margin:12px 0 12px 36px}
.chips{display:flex;gap:8px;overflow-x:auto;padding-bottom:4px;margin-bottom:16px;scrollbar-width:none}
.chips::-webkit-scrollbar{display:none}
.chip{background:#E5E5EA;border:none;padding:8px 16px;border-radius:20px;font-size:13px;font-weight:600;color:var(--tx);white-space:nowrap;cursor:pointer;transition:.2s}
.chip.act{background:var(--pri);color:#fff}
.tchip{background:#E5E5EA;border:2px solid transparent;padding:10px 16px;border-radius:20px;font-size:14px;font-weight:600;color:var(--tx);cursor:pointer;transition:.2s;display:inline-block;margin:0 6px 10px 0}
.tchip.act{background:#F0F8FF;color:var(--pri);border-color:var(--pri)}
.tap-area{text-align:center;padding:40px 20px}
.ic-gfx{width:180px;height:280px;background:var(--ic);border-radius:16px;margin:0 auto 32px;box-shadow:0 16px 32px rgba(46,49,146,.3);display:flex;flex-direction:column;justify-content:space-between;padding:24px 20px;color:#fff;animation:icfloat 3s ease-in-out infinite}
.ic-gfx .ic-mk{align-self:flex-end;width:32px;height:24px;background:rgba(255,255,255,.8);border-radius:4px}
.ic-gfx .ic-lg{font-size:20px;font-weight:800;font-style:italic;opacity:.9}
@keyframes icfloat{0%,100%{transform:translateY(0)}50%{transform:translateY(-10px)}}
.oac-hero{background:linear-gradient(135deg,#1A2A44,#2E5090 60%,#4A90D9);border-radius:var(--r-lg);padding:28px 20px;color:#fff;position:relative;overflow:hidden;margin-bottom:24px}
.oac-hero::before{content:'';position:absolute;top:-40px;right:-40px;width:140px;height:140px;border-radius:50%;background:rgba(255,255,255,.08)}
.oac-hero h3{font-size:20px;font-weight:800;margin-bottom:8px;line-height:1.4;position:relative;z-index:1}
.oac-hero p{font-size:13px;opacity:.85;line-height:1.5;position:relative;z-index:1}
.oac-ts{background:linear-gradient(135deg,var(--grn-bg),#F0F8FF);border:1px solid #BDE0FE;border-radius:var(--r-md);padding:16px;display:flex;align-items:center;gap:14px;margin-bottom:16px}
.oac-ts-i{width:48px;height:48px;border-radius:50%;background:var(--grn);display:flex;align-items:center;justify-content:center;color:#fff;flex-shrink:0;box-shadow:0 4px 12px rgba(52,199,89,.3)}
.oac-ts h4{font-size:18px;font-weight:800;margin-bottom:2px}
.oac-ts p{font-size:12px;color:var(--txs);line-height:1.4}
.oac-res{border-radius:var(--r-md);padding:20px;margin-bottom:16px;border:2px solid}
.oac-res.avl{background:var(--grn-bg);border-color:var(--grn)}
.oac-res.cnd{background:var(--org-bg);border-color:var(--org)}
.oac-res.una{background:var(--red-bg);border-color:var(--red)}
.oac-rb{display:inline-flex;align-items:center;gap:6px;padding:6px 12px;border-radius:20px;font-size:13px;font-weight:700;color:#fff;margin-bottom:12px}
.oac-co{background:var(--card);border:2px solid #E5E5EA;border-radius:var(--r-sm);padding:14px 16px;cursor:pointer;transition:.2s;margin-bottom:10px}
.oac-co.act{border-color:var(--pri);background:#F0F8FF}
.oac-sg{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px}
.oac-sb{border:2px solid #E5E5EA;background:var(--card);padding:12px;border-radius:var(--r-sm);font-size:14px;font-weight:700;cursor:pointer;transition:.2s;text-align:center}
.oac-sb.act{border-color:var(--pri);background:#F0F8FF;color:var(--pri)}
.bp-mock{background:#fff;border-radius:var(--r-md);border:2px dashed #BDE0FE;padding:20px;margin-bottom:24px;position:relative;overflow:hidden}
.bp-mock::before{content:'BOARDING PASS (PREVIEW)';position:absolute;top:8px;right:12px;font-size:9px;font-weight:700;color:#C7C7CC;letter-spacing:1px}
.bp-route{display:flex;align-items:center;gap:12px;margin:16px 0}
.bp-ap{text-align:center}
.bp-ap .code{font-size:28px;font-weight:800;letter-spacing:1px}
.bp-ap .nm{font-size:11px;color:var(--txs);font-weight:600}
.bp-arrow{flex:1;display:flex;align-items:center;justify-content:center;color:var(--pri)}
.succ{width:80px;height:80px;border-radius:50%;background:var(--grn);display:flex;align-items:center;justify-content:center;color:#fff;margin:0 auto 24px;box-shadow:0 8px 24px rgba(52,199,89,.4);animation:pop .5s cubic-bezier(.175,.885,.32,1.275)}
@keyframes pop{0%{transform:scale(0);opacity:0}100%{transform:scale(1);opacity:1}}
.fab{position:fixed;bottom:24px;right:calc(50% - 215px + 20px);width:64px;height:64px;border-radius:32px;background:#fff;color:var(--pri);display:flex;align-items:center;justify-content:center;box-shadow:0 8px 24px rgba(10,132,255,.35);cursor:pointer;z-index:100;transition:transform .2s;overflow:hidden;border:2px solid var(--pri)}
@media (max-width:430px){.fab{right:20px}}
.fab:active{transform:scale(.92)}
.fab-b{position:absolute;top:2px;right:2px;width:14px;height:14px;background:var(--red);border:2px solid #fff;border-radius:50%;z-index:2}
.sheet-ov{display:none;position:fixed;inset:0;background:rgba(0,0,0,.5);z-index:200;opacity:0;transition:opacity .3s;justify-content:center;align-items:flex-end}
.sheet-ov.open{display:flex;opacity:1}
.sheet{width:100%;max-width:430px;background:var(--bg);border-radius:24px 24px 0 0;display:flex;flex-direction:column;transform:translateY(100%);transition:transform .3s cubic-bezier(.175,.885,.32,1.1);max-height:85vh}
.sheet-ov.open .sheet{transform:translateY(0)}
.sheet.full{height:85vh}
.sheet-hd{padding:14px 20px;background:var(--card);border-radius:24px 24px 0 0;display:flex;justify-content:space-between;align-items:center;border-bottom:1px solid #E5E5EA;flex-shrink:0}
.sheet-hd h2{font-size:16px;font-weight:700;display:flex;align-items:center;gap:8px}
.close-b{background:#E5E5EA;border:none;width:32px;height:32px;border-radius:16px;display:flex;align-items:center;justify-content:center;cursor:pointer;color:var(--txs)}
.sheet-body{flex:1;overflow-y:auto;padding:16px 20px 24px}
.chat-msgs{flex:1;padding:20px;overflow-y:auto;display:flex;flex-direction:column;gap:16px}
.msg{max-width:88%;padding:12px 16px;border-radius:18px;font-size:14px;line-height:1.6;animation:fadeV .3s;word-wrap:break-word;overflow-wrap:break-word}
.msg-ai{background:var(--card);align-self:flex-start;border-bottom-left-radius:4px;box-shadow:var(--s-sm)}
.msg-usr{background:var(--pri);color:#fff;align-self:flex-end;border-bottom-right-radius:4px}
.msg-ai .chat-action{display:inline-block;margin-top:8px;padding:6px 12px;border-radius:16px;background:#F0F8FF;color:var(--pri);font-size:12px;font-weight:600;cursor:pointer;border:1px solid #BDE0FE}
.qprompts{display:flex;gap:8px;padding:12px 20px;overflow-x:auto;scrollbar-width:none}
.qprompts::-webkit-scrollbar{display:none}
.qp{background:var(--card);border:1px solid #E5E5EA;padding:8px 16px;border-radius:20px;font-size:13px;font-weight:600;color:var(--pri);white-space:nowrap;cursor:pointer;box-shadow:var(--s-sm)}
.chat-in{padding:12px 20px 24px;background:var(--card);border-top:1px solid #E5E5EA}
.chat-in .iw{display:flex;align-items:center;background:#F2F2F7;border-radius:24px;padding:4px 4px 4px 16px}
.chat-in input{flex:1;border:none;background:transparent;padding:10px 0;font-size:15px;outline:none}
.send-b{background:var(--pri);border:none;width:36px;height:36px;border-radius:18px;display:flex;align-items:center;justify-content:center;color:#fff;cursor:pointer}
.send-b:disabled{background:#C7C7CC}
.typing{display:flex;gap:4px;padding:12px 16px;align-self:flex-start}
.typing span{width:8px;height:8px;border-radius:50%;background:#C7C7CC;animation:bounce 1.4s infinite ease-in-out both}
.typing span:nth-child(1){animation-delay:-.32s}
.typing span:nth-child(2){animation-delay:-.16s}
@keyframes bounce{0%,80%,100%{transform:scale(0)}40%{transform:scale(1)}}
.toast{position:fixed;top:20px;left:50%;transform:translateX(-50%);background:rgba(0,0,0,.8);color:#fff;padding:12px 24px;border-radius:24px;font-size:14px;font-weight:600;z-index:1000;opacity:0;transition:opacity .3s;pointer-events:none}
.toast.show{opacity:1}
.ckb{width:22px;height:22px;accent-color:var(--pri);flex-shrink:0;cursor:pointer}
.step-c{width:28px;height:28px;border-radius:14px;background:#F0F8FF;color:var(--pri);display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:800;flex-shrink:0}
.wcard{color:#fff;border-radius:var(--r-md);margin:0 20px 16px;padding:14px 16px;display:flex;align-items:center;gap:14px;box-shadow:var(--s-sm);cursor:pointer;background:linear-gradient(135deg,#4A90D9,#7FB3E5)}
.wcard.sunny{background:linear-gradient(135deg,#FFA94D,#FFD166)}
.wcard.rainy{background:linear-gradient(135deg,#546E7A,#78909C)}
.wcard.snow{background:linear-gradient(135deg,#90A4AE,#CFD8DC);color:#263238}
.wcard .wi{font-size:40px;line-height:1}
.wcard .wbody{flex:1;min-width:0}
.wcard .wloc{font-size:11px;font-weight:600;opacity:.9;margin-bottom:2px}
.wcard .wt{font-size:24px;font-weight:800;display:flex;align-items:baseline;gap:6px}
.wcard .wt small{font-size:12px;font-weight:600;opacity:.9}
.wcard .wo{font-size:11px;margin-top:2px;opacity:.95;font-weight:600}
.wcard .wrange{font-size:11px;opacity:.9;font-weight:600;margin-top:2px}
.nsc{margin:0 20px 16px;background:var(--card);border-radius:var(--r-md);padding:14px 16px;box-shadow:var(--s-sm);border:1px solid #E5E5EA}
.nsc-hd{display:flex;justify-content:space-between;align-items:center;margin-bottom:8px}
.nsc-hd .t{font-size:13px;font-weight:700;display:flex;align-items:center;gap:6px;color:var(--pri-dk)}
.nsc-hd .more{font-size:11px;color:var(--pri);font-weight:600}
.nsc-scroll{display:flex;gap:10px;overflow-x:auto;scrollbar-width:none;padding-bottom:2px;margin:0 -4px;padding-left:4px}
.nsc-scroll::-webkit-scrollbar{display:none}
.nsc-item{flex:0 0 170px;background:#F9F9FB;border:1px solid #EAEAEE;border-radius:var(--r-sm);padding:10px 12px;cursor:pointer}
.nsc-item:active{transform:scale(.98)}
.nsc-item .nm{font-size:13px;font-weight:700;line-height:1.3;margin-bottom:4px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.nsc-item .ct{font-size:10px;font-weight:600;color:var(--pri);background:#F0F8FF;padding:2px 6px;border-radius:6px;display:inline-block;margin-bottom:4px}
.nsc-item .ds{font-size:11px;color:var(--txs);line-height:1.3}
.nsc-empty{font-size:12px;color:var(--txs);padding:6px 0;line-height:1.5}
.todo-card{background:var(--card);border:1px solid #E5E5EA;border-radius:var(--r-md);padding:14px;display:flex;gap:12px;margin-bottom:10px;cursor:pointer;align-items:center;transition:.15s}
.todo-card:active{transform:scale(.98)}
.todo-card.urgent{border-color:#FFC6C4;background:#FFFAFA}
.todo-card .sa-i{width:40px;height:40px;border-radius:12px;background:#F0F8FF;color:var(--pri);display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0}
.todo-card.urgent .sa-i{background:var(--red-bg);color:var(--red)}
.sa-body{flex:1;min-width:0}
.sa-body .t{font-size:14px;font-weight:700;margin-bottom:2px}
.sa-body .s{font-size:12px;color:var(--txs);line-height:1.3}
.sa-arrow{color:#C7C7CC;flex-shrink:0}
.empty-todo{background:var(--grn-bg);border:1px solid #BDE0FE;border-radius:var(--r-md);padding:20px 16px;text-align:center;color:var(--grn);font-weight:700;font-size:14px}
.wd-tabs{display:flex;gap:6px;background:#F2F2F7;padding:4px;border-radius:12px;margin-bottom:16px}
.wd-tab{flex:1;padding:8px;border:none;background:transparent;font-size:13px;font-weight:700;color:var(--txs);border-radius:8px;cursor:pointer}
.wd-tab.act{background:var(--card);color:var(--tx);box-shadow:var(--s-sm)}
.wd-hero{text-align:center;padding:16px 0 24px}
.wd-hero .ic{font-size:72px;line-height:1;margin-bottom:8px}
.wd-hero .tp{font-size:48px;font-weight:800;letter-spacing:-1px}
.wd-hero .cd{font-size:15px;color:var(--txs);font-weight:600;margin-top:4px}
.wd-row{display:flex;justify-content:space-between;padding:10px 0;border-bottom:1px solid #F2F2F7;font-size:13px}
.wd-row:last-child{border-bottom:none}
.wd-row span:first-child{color:var(--txs);font-weight:600}
.wd-row span:last-child{font-weight:700}
.wd-hour{display:flex;gap:10px;overflow-x:auto;padding-bottom:6px;scrollbar-width:none}
.wd-hour::-webkit-scrollbar{display:none}
.wd-hitem{flex:0 0 60px;text-align:center;background:#F9F9FB;border:1px solid #EAEAEE;border-radius:12px;padding:8px 4px}
.wd-hitem .h{font-size:11px;color:var(--txs);font-weight:600}
.wd-hitem .i{font-size:22px;margin:4px 0}
.wd-hitem .t{font-size:13px;font-weight:700}
.wd-day{display:flex;align-items:center;gap:10px;padding:10px 0;border-bottom:1px solid #F2F2F7}
.wd-day:last-child{border-bottom:none}
.wd-day .d{flex:0 0 60px;font-size:13px;font-weight:700}
.wd-day .i{font-size:22px;flex:0 0 30px}
.wd-day .c{flex:1;font-size:12px;color:var(--txs)}
.wd-day .r{font-size:13px;font-weight:700}
.sm-cat{display:inline-block;background:#F0F8FF;color:var(--pri);font-size:11px;font-weight:700;padding:4px 10px;border-radius:10px;margin-bottom:8px}
.sm-h{font-size:20px;font-weight:800;margin-bottom:6px}
.sm-sub{font-size:12px;color:var(--txs);margin-bottom:12px}
.sm-desc{font-size:13px;line-height:1.6;margin-bottom:16px;color:#333}
.sm-links{display:flex;flex-direction:column;gap:10px;margin-bottom:16px}
.sm-link{display:flex;align-items:center;gap:12px;padding:12px 14px;background:#F9F9FB;border:1px solid #EAEAEE;border-radius:var(--r-sm);text-decoration:none;color:var(--tx);font-size:14px;font-weight:600;cursor:pointer}
.sm-link:active{background:#F2F2F7}
.sm-link .ic{color:var(--pri);flex-shrink:0}
.sm-link .ar{margin-left:auto;color:#C7C7CC}
.login-bg{min-height:100vh;display:flex;flex-direction:column;align-items:center;justify-content:center;padding:40px 24px;background:linear-gradient(180deg,#F0F8FF 0%,#FFF 50%,#E5F9EB 100%)}
.login-logo{font-size:52px;font-weight:900;font-style:italic;color:var(--pri);letter-spacing:-1.5px;margin-bottom:8px;text-align:center;text-shadow:0 4px 16px rgba(10,132,255,.2)}
.login-logo sub{font-size:18px;color:var(--txs);font-style:normal;vertical-align:baseline;margin-left:4px}
.login-welcome{font-size:20px;font-weight:700;color:var(--tx);margin-bottom:24px;letter-spacing:.5px;text-align:center}
.login-form{width:100%;max-width:340px}
.login-chara{margin:0 auto 20px}
.mode-cat{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:12px}
.mode-cat button{border:2px solid #E5E5EA;background:var(--card);padding:10px 4px;border-radius:var(--r-sm);font-size:14px;font-weight:700;color:var(--tx);cursor:pointer;transition:.2s;text-align:center}
.mode-cat button.act{border-color:var(--pri);background:#F0F8FF;color:var(--pri)}
.mode-sub{display:grid;grid-template-columns:repeat(4,1fr);gap:6px;margin-bottom:16px}
.mode-sub button{border:2px solid #E5E5EA;background:var(--card);padding:10px 4px;border-radius:var(--r-sm);font-size:12px;font-weight:700;color:var(--tx);cursor:pointer;transition:.2s;text-align:center;display:flex;flex-direction:column;align-items:center;gap:2px}
.mode-sub button .em{font-size:20px;line-height:1}
.mode-sub button.act{border-color:var(--pri);background:#F0F8FF;color:var(--pri)}
.map-wrap{position:relative;margin-bottom:12px;border-radius:var(--r-md);overflow:hidden;box-shadow:var(--s-sm);background:#E5E5EA}
.map-wrap iframe{width:100%;height:340px;border:none;display:block}
.map-fallback{padding:40px 20px;text-align:center;background:#F9F9FB;min-height:200px;display:flex;flex-direction:column;justify-content:center;align-items:center;gap:10px}
.rc{background:var(--card);border-radius:var(--r-md);padding:16px;box-shadow:var(--s-sm);margin-bottom:12px;cursor:pointer;border:2px solid transparent;transition:.2s}
.rc:active{transform:scale(.98)}
.rc-hd{display:flex;align-items:center;gap:10px;margin-bottom:4px}
.rc-hd .em{font-size:22px}
.rc-hd .l{font-size:15px;font-weight:700}
.rc-sub{font-size:12px;color:var(--txs)}
.hub-opt{background:var(--card);border:2px solid #E5E5EA;border-radius:var(--r-md);padding:18px 16px;display:flex;align-items:center;gap:14px;cursor:pointer;margin-bottom:12px;transition:.2s}
.hub-opt:active{transform:scale(.98);border-color:var(--pri)}
.hub-opt .ic{width:48px;height:48px;border-radius:14px;background:#F0F8FF;color:var(--pri);display:flex;align-items:center;justify-content:center;flex-shrink:0}
.hub-opt .body{flex:1}
.hub-opt .body .t{font-size:15px;font-weight:700;margin-bottom:2px}
.hub-opt .body .s{font-size:12px;color:var(--txs)}
.ticket-card{background:var(--card);border:2px solid #E5E5EA;border-radius:var(--r-md);padding:14px;margin-bottom:10px;cursor:pointer;display:flex;gap:12px;align-items:center;transition:.15s}
.ticket-card:active{transform:scale(.99)}
.ticket-card.act{border-color:var(--pri);background:#F0F8FF}
.ticket-card.rec{border-color:var(--org);background:#FFFBF2}
.ticket-card .em{font-size:28px;flex-shrink:0;width:48px;height:48px;display:flex;align-items:center;justify-content:center;background:#F9F9FB;border-radius:12px}
.ticket-card.act .em{background:#fff}
.ticket-card .body{flex:1;min-width:0}
.ticket-card .body .t{font-size:14px;font-weight:700;margin-bottom:2px;display:flex;align-items:center;gap:6px}
.ticket-card .body .s{font-size:11px;color:var(--txs);line-height:1.3}
.ticket-card .body .p{font-size:14px;font-weight:800;color:var(--pri-dk);margin-top:4px}
.qty-row{display:flex;align-items:center;justify-content:space-between;padding:10px 0;border-bottom:1px solid #F2F2F7}
.qty-row:last-child{border-bottom:none}
.qty-row .l{font-size:14px;font-weight:700}
.qty-ctrl{display:flex;align-items:center;gap:12px}
.qty-ctrl button{width:32px;height:32px;border-radius:16px;border:1px solid #E5E5EA;background:var(--card);font-size:18px;font-weight:700;cursor:pointer;color:var(--tx)}
.qty-ctrl button:active{background:#F0F8FF}
.qty-ctrl .n{font-size:16px;font-weight:800;min-width:20px;text-align:center}
.chara-msg{display:flex;gap:10px;align-items:flex-start;background:#F0F8FF;border:1px solid #BDE0FE;border-radius:var(--r-md);padding:12px;margin-bottom:16px}
.chara-msg .chara{flex-shrink:0;width:44px;height:44px}
.chara-msg .bub{flex:1;font-size:13px;line-height:1.5;color:var(--pri-dk);font-weight:600}
.tour-free-text{width:100%;min-height:80px;background:#F2F2F7;border:1px solid #E5E5EA;padding:14px 16px;border-radius:var(--r-sm);font-size:14px;outline:none;color:var(--tx);font-weight:500;resize:vertical;font-family:inherit;line-height:1.6;margin-bottom:24px}
.tour-free-text::placeholder{color:var(--txs);font-weight:400}
.tour-free-text:focus{border-color:var(--pri);box-shadow:0 0 0 3px rgba(10,132,255,.12)}
.tour-loading{display:flex;flex-direction:column;align-items:center;justify-content:center;padding:60px 20px;text-align:center}
.tour-loading .tl-spinner{width:48px;height:48px;border:4px solid #E5E5EA;border-top-color:var(--pri);border-radius:50%;animation:tlspin 1s linear infinite;margin-bottom:20px}
@keyframes tlspin{to{transform:rotate(360deg)}}
.tour-loading .tl-msg{font-size:15px;font-weight:700;color:var(--tx);margin-bottom:6px}
.tour-loading .tl-sub{font-size:12px;color:var(--txs)}
.tour-ai-card{background:var(--card);border-radius:var(--r-md);padding:16px;box-shadow:var(--s-sm);margin-bottom:12px;cursor:pointer;border:2px solid transparent;transition:.2s}
.tour-ai-card:active{transform:scale(.98)}
.tour-ai-card.top{border-color:var(--pri);background:linear-gradient(135deg,#F0F8FF,#FFF)}
.tour-ai-card .tac-head{display:flex;align-items:center;gap:10px;margin-bottom:8px}
.tour-ai-card .tac-head .em{font-size:22px}
.tour-ai-card .tac-head .l{font-size:15px;font-weight:700;flex:1}
.tour-ai-card .tac-reason{font-size:12px;color:var(--pri-dk);background:#F0F8FF;border:1px solid #BDE0FE;border-radius:8px;padding:8px 12px;line-height:1.5;margin-bottom:8px}
.tour-ai-card .tac-meta{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:6px}
.tour-ai-card .tac-spots{font-size:12px;color:var(--txs)}
/* ===== AI Next-Action Cards (Home) ===== */
.ai-next{margin:0 20px 16px}
.ai-next-hd{display:flex;align-items:center;gap:8px;margin-bottom:10px;padding:0 2px}
.ai-next-hd .ai-chara{flex-shrink:0}
.ai-next-hd .ai-label{font-size:14px;font-weight:700;color:var(--pri-dk);flex:1}
.ai-next-hd .ai-dots{display:flex;gap:5px;align-items:center}
.ai-dot{width:6px;height:6px;border-radius:3px;background:#C7C7CC;border:none;padding:0;cursor:pointer;transition:all .3s ease;flex-shrink:0}
.ai-dot.act{background:var(--pri);width:16px}
.ai-carousel{position:relative;overflow:hidden;border-radius:var(--r-md)}
.ai-carousel-track{display:flex;transition:transform .4s cubic-bezier(.4,0,.2,1);will-change:transform}
.ai-carousel-slide{flex:0 0 100%;min-width:0;padding:0 1px}
.ai-card{background:var(--card);border-radius:var(--r-md);padding:14px;box-shadow:var(--s-sm);border-left:4px solid var(--pri);transition:.15s}
.ai-card:active{transform:scale(.99)}
.ai-card.emergency{border-left-color:var(--red)}
.ai-card.warn{border-left-color:var(--org)}
.ai-card-row{display:flex;align-items:flex-start;gap:12px}
.ai-card-icon{width:38px;height:38px;border-radius:12px;background:#F0F8FF;color:var(--pri);display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0}
.ai-card.emergency .ai-card-icon{background:var(--red-bg);color:var(--red)}
.ai-card.warn .ai-card-icon{background:var(--org-bg);color:var(--org)}
.ai-card-body{flex:1;min-width:0}
.ai-card-title{font-size:14px;font-weight:700;margin-bottom:2px;display:flex;align-items:center;gap:6px}
.ai-card-summary{font-size:12px;color:var(--txs);line-height:1.4;margin-bottom:8px}
.ai-card-badge{display:inline-block;font-size:10px;font-weight:700;padding:2px 8px;border-radius:8px;background:#F0F8FF;color:var(--pri);border:1px solid #BDE0FE}
.ai-card.emergency .ai-card-badge{background:var(--red-bg);color:var(--red);border-color:#FFC6C4}
.ai-card.warn .ai-card-badge{background:var(--org-bg);color:var(--org);border-color:#FFE0B2}
.ai-action-btn{border:none;background:var(--pri);color:#fff;font-size:12px;font-weight:700;padding:8px 16px;border-radius:var(--r-sm);cursor:pointer;transition:.15s;margin-top:6px;display:inline-block}
.ai-action-btn:active{opacity:.8;transform:scale(.97)}
.ai-action-btn.secondary{background:#F0F8FF;color:var(--pri);border:1px solid #BDE0FE}
/* ===== Chat AI Cards (inside chat) ===== */
.chat-card-list{display:flex;flex-direction:column;gap:8px;margin-top:10px}
.chat-ai-card{background:#F9F9FB;border:1px solid #EAEAEE;border-radius:var(--r-sm);padding:12px;border-left:3px solid var(--pri)}
.chat-ai-card .cac-title{font-size:13px;font-weight:700;margin-bottom:4px;display:flex;align-items:center;gap:6px}
.chat-ai-card .cac-summary{font-size:12px;color:var(--txs);line-height:1.4;margin-bottom:8px}
.chat-ai-card .cac-badge{display:inline-block;font-size:10px;font-weight:600;padding:2px 6px;border-radius:6px;background:#F0F8FF;color:var(--pri);margin-bottom:6px}
.chat-ai-card .cac-btn{border:none;background:var(--pri);color:#fff;font-size:12px;font-weight:700;padding:7px 14px;border-radius:8px;cursor:pointer}
/* ===== Hierarchical Menu ===== */
.side-menu nav .menu-group-hd{display:flex;align-items:center;justify-content:space-between;padding:14px 20px;font-size:15px;font-weight:600;color:var(--tx);cursor:pointer;transition:background .15s}
.side-menu nav .menu-group-hd:active{background:#F0F8FF}
.side-menu nav .menu-group-hd svg:first-child{width:22px;height:22px;color:var(--txs);flex-shrink:0;margin-right:14px}
.side-menu nav .menu-group-hd.cur{background:#F0F8FF;color:var(--pri)}
.side-menu nav .menu-group-hd.cur svg:first-child{color:var(--pri)}
.menu-expand-icon{width:16px;height:16px;color:var(--txs);transition:transform .2s;flex-shrink:0}
.menu-expand-icon.open{transform:rotate(90deg)}
.menu-children{overflow:hidden;max-height:0;transition:max-height .25s ease}
.menu-children.open{max-height:200px}
.menu-children a{display:flex;align-items:center;gap:10px;padding:11px 20px 11px 56px;font-size:13px;font-weight:600;color:var(--txs);text-decoration:none;cursor:pointer;transition:background .15s}
.menu-children a:active,.menu-children a.cur{background:#F0F8FF;color:var(--pri)}
/* ===== History Views ===== */
.hist-card{background:var(--card);border-radius:var(--r-md);padding:14px;box-shadow:var(--s-sm);margin-bottom:12px;cursor:pointer;border:1px solid #E5E5EA;transition:.15s}
.hist-card:active{transform:scale(.98)}
.hist-card .hc-hd{display:flex;align-items:center;gap:10px;margin-bottom:6px}
.hist-card .hc-hd .em{font-size:22px}
.hist-card .hc-hd .t{font-size:14px;font-weight:700;flex:1}
.hist-card .hc-hd .dt{font-size:11px;color:var(--txs);font-weight:600;flex-shrink:0}
.hist-card .hc-body{font-size:12px;color:var(--txs);line-height:1.4}
.hist-card .hc-tags{display:flex;flex-wrap:wrap;gap:4px;margin-top:6px}
.hist-empty{background:var(--card);border-radius:var(--r-md);padding:32px 20px;text-align:center;box-shadow:var(--s-sm)}
.hist-empty .em{font-size:40px;margin-bottom:12px}
.hist-empty .t{font-size:14px;font-weight:700;margin-bottom:4px}
.hist-empty .s{font-size:12px;color:var(--txs)}
.hist-del-btn{border:none;background:var(--red-bg);color:var(--red);font-size:12px;font-weight:700;padding:8px 16px;border-radius:var(--r-sm);cursor:pointer;margin-top:12px}
.hist-del-btn:active{opacity:.7}
/* ===== Avatar System ===== */
.avatar-sel-wrap{margin-top:20px;width:100%;max-width:380px}
.avatar-sel-title{font-size:15px;font-weight:700;text-align:center;margin-bottom:4px;color:var(--tx)}
.avatar-sel-sub{font-size:12px;color:var(--txs);text-align:center;margin-bottom:16px}
.avatar-cards{display:flex;gap:10px;overflow-x:auto;padding:4px 0 8px;scrollbar-width:none}
.avatar-cards::-webkit-scrollbar{display:none}
.av-card{flex:0 0 120px;background:var(--card);border:3px solid #E5E5EA;border-radius:var(--r-md);padding:10px 8px 12px;text-align:center;cursor:pointer;transition:.25s;position:relative;overflow:hidden}
.av-card:active{transform:scale(.96)}
.av-card.sel{border-color:var(--pri);box-shadow:0 4px 16px rgba(0,0,0,.12)}
.av-card .av-img{width:80px;height:80px;border-radius:50%;object-fit:cover;margin:0 auto 8px;display:block;border:3px solid #E5E5EA;transition:.2s}
.av-card.sel .av-img{border-color:var(--pri)}
.av-card .av-nm{font-size:14px;font-weight:800;margin-bottom:2px}
.av-card .av-desc{font-size:10px;color:var(--txs);line-height:1.3}
.av-card .av-check{position:absolute;top:6px;right:6px;width:22px;height:22px;border-radius:50%;background:var(--pri);color:#fff;display:none;align-items:center;justify-content:center;font-size:12px;font-weight:700}
.av-card.sel .av-check{display:flex}
/* FAB avatar */
.fab{overflow:visible}
.fab-avatar{width:56px;height:56px;border-radius:50%;object-fit:cover;display:block;position:relative;z-index:1}
.fab-mood{position:absolute;top:-2px;right:-2px;width:22px;height:22px;border-radius:50%;background:#fff;border:2px solid var(--pri);display:none;align-items:center;justify-content:center;font-size:12px;z-index:3;box-shadow:0 2px 6px rgba(0,0,0,.15)}
.fab-b{display:none}
/* Chat avatar */
.chat-av-hd{display:flex;align-items:center;gap:8px}
.chat-av-img{width:32px;height:32px;border-radius:50%;object-fit:cover;border:2px solid rgba(255,255,255,.3)}
/* Avatar mood halo on FAB */
@keyframes moodPulse{0%,100%{box-shadow:0 0 0 0 var(--mood-halo)}50%{box-shadow:0 0 0 8px transparent}}
.fab.mood-active{animation:moodPulse 2s ease-in-out infinite}
/* Settings avatar picker */
.settings-av-row{display:flex;gap:10px;margin-bottom:16px;overflow-x:auto;padding-bottom:4px;scrollbar-width:none}
.settings-av-row::-webkit-scrollbar{display:none}
.settings-av-opt{flex:0 0 90px;text-align:center;cursor:pointer;padding:8px;border:2px solid #E5E5EA;border-radius:var(--r-sm);transition:.2s;background:var(--card)}
.settings-av-opt.act{border-color:var(--pri);background:#F0F8FF}
.settings-av-opt img{width:60px;height:60px;border-radius:50%;object-fit:cover;margin-bottom:4px}
.settings-av-opt .nm{font-size:12px;font-weight:700}
/* Chara msg avatar override */
.chara-av{width:44px;height:44px;border-radius:50%;object-fit:cover;flex-shrink:0;border:2px solid var(--pri)}
/* ===== RPG Welcome Screen ===== */
.rpg-overlay{position:fixed;inset:0;z-index:500;display:flex;flex-direction:column;align-items:center;justify-content:flex-end;opacity:0;pointer-events:none;transition:opacity .5s}
.rpg-overlay.active{opacity:1;pointer-events:auto}
.rpg-bg{position:absolute;inset:0;background:linear-gradient(180deg,#0a0e27 0%,#0d1235 20%,#1a1a4e 45%,#2e3192 70%,#4a6cf7 100%);overflow:hidden}
.rpg-stars{position:absolute;inset:0}
.rpg-star{position:absolute;width:2px;height:2px;background:#fff;border-radius:50%;animation:rpgTwinkle 2s ease-in-out infinite}
@keyframes rpgTwinkle{0%,100%{opacity:.2;transform:scale(.8)}50%{opacity:1;transform:scale(1.3)}}
.rpg-chara-wrap{position:absolute;z-index:2;left:50%;bottom:170px;transform:translateX(-50%) translateY(80px);opacity:0;animation:rpgCharaIn 1s .3s cubic-bezier(.175,.885,.32,1.275) forwards;pointer-events:none}
@keyframes rpgCharaIn{to{opacity:1;transform:translateX(-50%) translateY(0)}}
.rpg-chara-wrap img{display:block;height:62vh;max-height:520px;width:auto;object-fit:contain;filter:drop-shadow(0 0 60px rgba(10,132,255,.4)) drop-shadow(0 0 120px rgba(46,49,146,.3))}
.rpg-chara-wrap.is-jpg img{height:55vh;max-height:460px;border-radius:24px;-webkit-mask-image:linear-gradient(to bottom,black 60%,transparent 100%);mask-image:linear-gradient(to bottom,black 60%,transparent 100%)}
.rpg-chara-glow{position:absolute;bottom:-30px;left:50%;transform:translateX(-50%);width:200px;height:80px;background:radial-gradient(ellipse,rgba(10,132,255,.35) 0%,transparent 70%);border-radius:50%;pointer-events:none}
.rpg-dialog{position:relative;z-index:3;width:100%;max-width:430px;background:linear-gradient(180deg,rgba(0,0,0,.6),rgba(0,0,0,.85) 30%);backdrop-filter:blur(16px);border-top:2px solid rgba(255,255,255,.15);padding:20px 28px 28px;min-height:160px;display:flex;flex-direction:column}
.rpg-name{color:#7EB8FF;font-size:13px;font-weight:800;margin-bottom:6px;letter-spacing:1px;text-shadow:0 0 12px rgba(126,184,255,.4)}
.rpg-text{color:#fff;font-size:16px;line-height:1.8;font-weight:500;min-height:56px;white-space:pre-wrap;text-shadow:0 1px 4px rgba(0,0,0,.5)}
.rpg-cursor{display:inline-block;width:8px;height:2px;background:#7EB8FF;animation:rpgBlink 1s step-end infinite;vertical-align:middle;margin-left:4px}
@keyframes rpgBlink{0%,100%{opacity:1}50%{opacity:0}}
.rpg-tap{color:rgba(255,255,255,.5);font-size:12px;font-weight:600;text-align:center;margin-top:12px;animation:rpgPulse 1.5s ease-in-out infinite}
@keyframes rpgPulse{0%,100%{opacity:.4}50%{opacity:.9}}
.rpg-skip{position:absolute;top:16px;right:20px;z-index:4;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.15);color:rgba(255,255,255,.5);font-size:12px;font-weight:600;padding:6px 14px;border-radius:16px;cursor:pointer;backdrop-filter:blur(4px)}
.rpg-skip:active{background:rgba(255,255,255,.2)}
</style>
</head>
<body>
<div class="app" id="app">
<div class="g-hdr" id="gHdr">
  <button class="ham" id="hamBtn" aria-label="Menu"><span></span><span></span><span></span></button>
  <div class="logo" onclick="nav('home')">AssisTrip<sub>AI</sub></div>
  <span class="admin-badge" id="adminBadge" style="display:none">Admin</span>
</div>
<div id="adminTabBar" class="admin-tabs" style="display:none">
  <button class="atab act" id="atabMain" onclick="switchAdminTab('main')">メイン</button>
  <button class="atab" id="atabAdmin" onclick="switchAdminTab('admin')">管理者設定</button>
</div>
<div class="menu-overlay" id="menuOv"></div>
<div class="side-menu" id="sideMenu">
  <header><div class="logo" onclick="nav('home')">AssisTrip<sub>AI</sub></div></header>
  <nav id="menuNav"></nav>
</div>
<div id="v-login" class="view"></div>
<div id="v-profile-setup" class="view"></div>
<div id="v-settings" class="view"></div>
<div id="v-admin-settings" class="view"></div>
<div id="v-home" class="view active">
  <div id="homeGreeting"></div>
  <div id="homeWeather"></div>
  <div id="homeAI"></div>
  <div id="homeNearby"></div>
  <section class="sec">
    <div class="pay-card" onclick="nav('pay-top')">
      <div class="fx jcsb aic mb4"><span class="fw7 fx aic g2"><svg width="24" height="24" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="5" width="20" height="14" rx="2"/><path d="M2 10h20"/></svg>交通・決済</span><span class="pay-status">連携済み</span></div>
      <div class="pay-label">IC残高 (Balance)</div>
      <div class="pay-bal js-bal">¥ 4,500</div>
      <div class="btn-row" style="pointer-events:auto"><button class="btn bp" onclick="event.stopPropagation();nav('charge')">チャージ</button><button class="btn bs" onclick="event.stopPropagation();nav('tap')">かざして使う</button></div>
    </div>
  </section>
  <section class="sec">
    <div class="sec-t">ToDoリスト <small>ToDo List</small></div>
    <div id="todoList"></div>
  </section>
  <section class="sec">
    <div class="sec-t">サービス <small>Quick Access</small></div>
    <div class="qgrid" id="quickGrid"></div>
  </section>
  <section class="sec">
    <div class="ml" id="homeLinks"></div>
  </section>
</div>
<div id="v-pay-top" class="view"></div>
<div id="v-charge" class="view"></div>
<div id="v-tap" class="view"></div>
<div id="v-ic-manage" class="view"></div>
<div id="v-mobility-hub" class="view"></div>
<div id="v-mobility" class="view"></div>
<div id="v-ticket" class="view"></div>
<div id="v-ticket-confirm" class="view"></div>
<div id="v-ticket-complete" class="view"></div>
<div id="v-todo-detail" class="view"></div>
<div id="v-baggage" class="view"></div>
<div id="v-bag-form" class="view"></div>
<div id="v-bag-confirm" class="view"></div>
<div id="v-bag-complete" class="view"></div>
<div id="v-tour" class="view"></div>
<div id="v-tour-results" class="view"></div>
<div id="v-tour-detail" class="view"></div>
<div id="v-trouble" class="view"></div>
<div id="v-trouble-detail" class="view"></div>
<div id="v-refund" class="view"></div>
<div id="v-refund-form" class="view"></div>
<div id="v-refund-confirm" class="view"></div>
<div id="v-refund-complete" class="view"></div>
<div id="v-oac" class="view"></div>
<div id="v-oac-form" class="view"></div>
<div id="v-oac-confirm" class="view"></div>
<div id="v-oac-complete" class="view"></div>
<div id="v-history-hub" class="view"></div>
<div id="v-history-tours" class="view"></div>
<div id="v-history-tour-detail" class="view"></div>
<div id="v-history-baggage" class="view"></div>
<div id="v-history-baggage-detail" class="view"></div>
<div id="v-history-tickets" class="view"></div>
<div id="v-history-refunds" class="view"></div>
<div id="v-history-oac" class="view"></div>
<div class="fab" id="chatFab"><img class="fab-avatar" id="fabAvatarImg" src="" alt="Guide"><div class="fab-mood" id="fabMood"></div></div>
</div>
<div class="sheet-ov" id="sheetOv">
  <div class="sheet" id="sheetBox" onclick="event.stopPropagation()">
    <div class="sheet-hd"><h2 id="sheetTitle"></h2><button class="close-b" onclick="closeSheet()"><svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M18 6L6 18M6 6l12 12"/></svg></button></div>
    <div class="sheet-body" id="sheetBody"></div>
  </div>
</div>
<div class="sheet-ov" id="chatOv">
  <div class="sheet full" onclick="event.stopPropagation()">
    <div class="sheet-hd"><h2><div class="chat-av-hd"><img class="chat-av-img" id="chatAvatarImg" src=""><span>AI コンシェルジュ<small style="font-weight:500;font-size:11px;color:var(--txs);margin-left:4px" id="chatAvatarName"></small></span></div></h2><button class="close-b" id="chatClose"><svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M18 6L6 18M6 6l12 12"/></svg></button></div>
    <div class="chat-msgs" id="chatMsgs"></div>
    <div class="qprompts"><div class="qp" onclick="qMsg('新宿駅への行き方は？')">新宿駅への行き方は？</div><div class="qp" onclick="qMsg('近くのおすすめスポットは？')">近くのおすすめスポットは？</div><div class="qp" onclick="qMsg('今日の天気に合う服装は？')">今日の服装は？</div></div>
    <div class="chat-in"><div class="iw"><input id="chatIn" placeholder="メッセージを入力..."><button class="send-b" id="sendB" disabled><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 2L11 13M22 2l-7 20-4-9-9-4 20-7z"/></svg></button></div></div>
  </div>
</div>
<div class="toast" id="toast"></div>
<script>
/* ── Admin Settings: localStorage helpers ── */
const ADMIN_KEYS = {
  isAdmin:        'assisTripIsAdmin',
  aiProvider:     'assisTripAiProvider',
  openAiApiKey:   'assisTripOpenAiApiKey',
  geminiApiKey:   'assisTripGeminiApiKey',
  claudeApiKey:   'assisTripClaudeApiKey',
  googleMapsApiKey:'assisTripGoogleMapsApiKey',
  aiSystemPrompt: 'assisTripAiSystemPrompt',
  lastSaved:      'assisTripAdminLastSavedAt',
  avatar:         'assisTripAvatarId'
};
function getAdminSetting(key, fallback){
  try{ const v=localStorage.getItem(ADMIN_KEYS[key]); return v!==null?v:fallback; }catch(e){ return fallback; }
}
function setAdminSetting(key, val){
  try{ localStorage.setItem(ADMIN_KEYS[key], val); }catch(e){}
}
function isAdminMode(){ return getAdminSetting('isAdmin','false')==='true'; }
function setAdminMode(v){ setAdminSetting('isAdmin', v?'true':'false'); }

/* ── Records (History) Management ── */
const RECORDS_KEY = 'assisTripRecords';
function loadRecords(){
  try{ const d=localStorage.getItem(RECORDS_KEY); return d?JSON.parse(d):{tours:[],baggage:[],tickets:[],refunds:[],oac:[]}; }
  catch(e){ return {tours:[],baggage:[],tickets:[],refunds:[],oac:[]}; }
}
function saveRecords(records){ try{ localStorage.setItem(RECORDS_KEY,JSON.stringify(records)); }catch(e){} }
function addRecord(category,record){
  const records=loadRecords();
  if(!records[category]) records[category]=[];
  record.id=record.id||'rec_'+Date.now()+'_'+Math.random().toString(36).slice(2,6);
  record.savedAt=record.savedAt||new Date().toISOString();
  records[category].unshift(record);
  saveRecords(records);
  return record;
}
function deleteRecord(category,id){
  const records=loadRecords();
  if(!records[category]) return;
  records[category]=records[category].filter(r=>r.id!==id);
  saveRecords(records);
}
function fmtSavedDate(iso){
  if(!iso) return '';
  const d=new Date(iso);
  return d.getFullYear()+'/'+(d.getMonth()+1)+'/'+d.getDate()+' '+String(d.getHours()).padStart(2,'0')+':'+String(d.getMinutes()).padStart(2,'0');
}



/* ── Avatar System ── */
const AVATAR_KEY='assisTripAvatar';
const AVATARS=[
  {
    id:'samurai',name:'武蔵（むさし）',
    desc:'力強く頼もしい案内役。迷った時にズバッと答えを示してくれます。',
    shortDesc:'頼れる武将ガイド',
    img:'data:image/jpeg;base64,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',
    imgSm:'data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAsICAoIBwsKCQoNDAsNERwSEQ8PESIZGhQcKSQrKigkJyctMkA3LTA9MCcnOEw5PUNFSElIKzZPVU5GVEBHSEX/2wBDAQwNDREPESESEiFFLicuRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUX/wAARCAAuAFADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwCjFCcDNX7eAEc8GmwKCea0YIgFBArIpDUh+TAGf6VNHbHBJqzEinHbNSsNqkZwexpDMyHy1a7R2fdHICAR2bHT1Gf51XuLqNnSOJyS8gjKqOc9T+QrHstXbVfEdxawyW8q28TKk8hKh+RnO3r/ACrIutUj07WFMghCTKyebCS3lDdyQD0ORmps72L6XO4MGcnHWopIQqYxzV2AK1vHiXzQVBEnHzj14pWjD8VRJiNBxk1SMe53c/QVt3KbVYjp2rOniKQgDuaYieLjHHNacDgr0rLgfjmtK3IIPpSYFtTgcdcVk+JNSax0svFIiTM2AGAOR3wD7VqLyuSTXAeLL9ZdScbgyRRtCinP3z94/wAh+dOO4nsMj02TRrtdQtmU74xIoA27dwHBA44/Ks+LS5te1Fi0o83mRiQDgD2FbN5MiwQ4untnMSsSFzuHABOD69Mcms2x1JbNpyZxOHjwYwCueQc57VV9L9SnGz8vX+mdL4Q1WW8Se2mkUiDHkqFCnZyD0/CujZwM4rynRdQNjqUV2CVEbkSAD70ZPP5V6aXDgFTkEZz61MtxIjuHBwtUrokleemanuJAo7Z6VRmmzkegpAJDIcdavwTH14rIhkO0Y9KtwsTz6UAbiTADHeuF12EQ6i8cSr5odjycfI/Gc+oyfyrqI5mK1j6vPHDqcM0kZfy4+xxnJyM+oFCunoUknozkr50nnYszCOL92rAZGB3APvVVJo12sjFpd/DYxxz+eRVqW4EivLGXXexwh6AE5/On6dAkqSyYxLHyhHGD71tb3bmOvNYnsbaS5ZLAffkY9V5SPJJJ/M13e8RqqoQFUYH0rz3ZPHeNdvKz8M7bXKNjqcEd/wBK6O2eVESUXc0sUiZVJgpIz7ispGqL9zcYfGaotOWc5PJGKiuJTnJqo7knJoQmf//Z',
    theme:{pri:'#1B3A5C',priDk:'#0F2640',accent:'#C5A55A',bg:'#F0EDE6',cardGrad:'linear-gradient(135deg,#1B3A5C,#2E5A8A)',fabRing:'#C5A55A',chatHd:'#1B3A5C',greetEmoji:'⚔️'},
    tone:'武将のように頼もしく、端的で判断力がある口調。「〜でござる」は使わず、落ち着いた敬語で力強く案内する。「任せろ」「迷う必要はない」のような後押しが得意。',
    greet:'よく参った。この武蔵が、旅の道案内を務めよう。'
  },
  {
    id:'sakura',name:'さくら',
    desc:'上品で丁寧な案内役。観光の提案が得意で、きめ細やかにサポートします。',
    shortDesc:'やさしい和装ガイド',
    img:'data:image/jpeg;base64,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',
    imgSm:'data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAsICAoIBwsKCQoNDAsNERwSEQ8PESIZGhQcKSQrKigkJyctMkA3LTA9MCcnOEw5PUNFSElIKzZPVU5GVEBHSEX/2wBDAQwNDREPESESEiFFLicuRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUX/wAARCAAuAFADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwDsQvFSLSIM08DoMViBIoNPBZehP4UsSgnDcClOBnB78ZFMDB8Q6wNItxNv2AZBJXI6dQO5BA496yvDvimTWrx12s8YOFwACM8cgccdc+9bOr6N9s1K0v8AzQFtVcGIruVicYOM4OCO9ZWh6Qt1r8uspIyLEzxeWFCqxxg8D0457/hS0vYu3u3Op2FiAOSaY+7o2eOOamK1G6kjP4UySLAyGf5gTyAeaQAdhgU7inSbN42A4x3pAMwFk2o4cY6gEVLuyMA9evvVWP73PH1qzFjcM8CgRKnTrSyvHFG0khCooySewporI8UfPpPlox+eVQOOuMnH6U/UdrmWdRv7nUPMd0UQsxWItsUD/wBm4PX3rEXWPsur3F1ag2kYBOAeGHYMO+ev4morGCOKzb7VslcSsrb1JYDAx17DOMVkapNHcqsMKofnACIhAPNZuScrWOhQSje56xpWopqmmwXSYy6/MAeFbuKsNxkjtXIeApSYtTRi24TISG7Erz/L8q6xiTgDkk8CrZziFSOdpAboTTQTmkluHbAdshOAPSoxIecd6AHwsiujfMT/ABZ9anlaMsPL9OaoRtgVOpouFyxnA5PNYHjOaOHw9I0i7suuF7nr098VuZz0rkvHk7w/2YCkUsAlaR4pF3LIQBgEenNNbgYNreR3EDy3Uk0ErYG6HEqkYGCeM57VIun3S20lxpqTXtwEILZVFQE8sM4PSs/Sdt3HggRRBdwVEBbntuPWnavcvZWgjiuLjy3OWQMFDYPfHP61nL4rHSk/Z83yN/4cTLJZaixOZWmUtlgc8Hn6V17uQcg4x71514H1SWTXrmNC62t4jzCFn3bGyDnPc+9d+mx5cS7tuMnb1q3uc41pgWyTn60ocdqoySDzDsBC9gaekhpCZ//Z',
    theme:{pri:'#B5678E',priDk:'#8E4466',accent:'#D4A574',bg:'#FBF5F0',cardGrad:'linear-gradient(135deg,#B5678E,#D4A0B9)',fabRing:'#D4A574',chatHd:'#B5678E',greetEmoji:'🌸'},
    tone:'上品で丁寧な口調。「〜ですね」「いかがでしょうか」のような柔らかい提案型。観光や文化の案内に深みを持たせる。落ち着きがあり、安心感を与える話し方。',
    greet:'ようこそ日本へ。わたくし、さくらがお供いたします。'
  },
  {
    id:'ponta',name:'ぽん太',
    desc:'親しみやすいカジュアルガイド。気軽に何でも相談できます。',
    shortDesc:'フレンドリーなたぬきガイド',
    img:'data:image/jpeg;base64,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',
    imgSm:'data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAsICAoIBwsKCQoNDAsNERwSEQ8PESIZGhQcKSQrKigkJyctMkA3LTA9MCcnOEw5PUNFSElIKzZPVU5GVEBHSEX/2wBDAQwNDREPESESEiFFLicuRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUVFRUX/wAARCAAuAFADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwDrQKkU8VCZAGCnv2FA3ZyDg+p7VysC0Rkdce9NedIYHlndY0jGXZjgLRDkjBbPvTbu1S6t5oJADHMpUj6/5zTQxJry3hiWSSeNEcZViww309abBfW1022C4jkOM4Vs8VwMXiKNLGxsJUja6tC0LzTAkIu7rjvwP0qjD4oEWoXksaR7WhdIWUbSoI6EA4yPWmOyPTknjnj8yGRZEOcMhBBqIQ4OeSWPJJqLRbJbHRrSEdRGGY+rEZJ/M1ZkYcrkf1qWITGOOwpyjApgkwVG4AHjJ6GpP4gKAKsT4ZmbpnFTNKvAP3j0FZqXXILEDjITPfp/WrW9YmDzcl+FAHpU3GX1IVNxAJo2EnLvk9cDpUEUjY3SYXIyFAycVKsqu3uPUVSA818UaKbfxLM8IIiuB5uB2z979azdE0pL3V7aJxiJ5lDDH8I5xXZeJC4vw3GCpjz6DqP61gWrtaX0ciBQ0bLtOfUincq2h6awJXCnb+FU5Q+75irf7x4FTO7ZIXg9smqrAvIyO2WAB5pNkghRidu0+rDp/wDqqSNdjfxYPQZ6VDJIlvHlmGPTIAqImUQyb5PnJ4H5cUgMp5pFkRiuVAyTxxwff9KfJeK4BlJwygABydvH8/pWE1xLNEG3EAc9eevX6+9JBK0QeaRjKykplu2PaoT0Fc6tdT3NlQ4yoBJI2rVyG/jdgFI44JPH/wCuuXt7jCrO2SuQGA6nJq/p8cc4CspO7LdcfypKTGUvEV0gvDnaUBBJ78isSQoEkkYDauAwPpXTS6LdXOuRXatbx29sCEX5mZz2LfnVLW/DVxeI8sFxEkhPzjZtVv581rYrm0sdBaalaX1sHt51fYAGPQg470y6n3EqpBDcdfQ9P1rB0jwlLpV1HdnUWfEe1ogmFbI9c0srkfvAx8sAnHcVMtCTTubkpnzSpgIIdSOR78daqf2nEzK6E7FUFH6k56r+mfwrPnuEkldXUsFOMnqfrWe0w2srF94ICsO3PU0ribP/2Q==',
    theme:{pri:'#5B8C3E',priDk:'#3E6B28',accent:'#C4A265',bg:'#F5F3ED',cardGrad:'linear-gradient(135deg,#5B8C3E,#7FB356)',fabRing:'#C4A265',chatHd:'#5B8C3E',greetEmoji:'🍃'},
    tone:'フレンドリーでカジュアルな口調。「〜だよ！」「〜してみない？」のような親しみやすい話し方。絵文字を少し多めに使い、会話を楽しくする。気軽さ重視。',
    greet:'やぁ！ぽん太だよ〜！一緒に楽しい旅にしよう！'
  },
  {
    id:'tsumugi',name:'つむぎ',
    desc:'旅行者専用の頼れるAIコンシェルジュ。日本の旅を隅々までサポートします。',
    shortDesc:'旅のAIコンシェルジュ',
    img:"data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='120' height='120' viewBox='0 0 64 64'%3E%3Cdefs%3E%3CradialGradient id='bg' cx='50%25' cy='45%25' r='50%25'%3E%3Cstop offset='0' stop-color='%23E8F4FD'/%3E%3Cstop offset='1' stop-color='%23D0E8FF'/%3E%3C/radialGradient%3E%3CradialGradient id='sk' cx='45%25' cy='38%25' r='55%25'%3E%3Cstop offset='0' stop-color='%23FFF0E6'/%3E%3Cstop offset='.6' stop-color='%23FFE0C9'/%3E%3Cstop offset='1' stop-color='%23F5CBA7'/%3E%3C/radialGradient%3E%3ClinearGradient id='hr' x1='0' y1='0' x2='0' y2='1'%3E%3Cstop offset='0' stop-color='%233D2B1F'/%3E%3Cstop offset='1' stop-color='%23241A12'/%3E%3C/linearGradient%3E%3ClinearGradient id='cp' x1='0' y1='0' x2='1' y2='1'%3E%3Cstop offset='0' stop-color='%231E90FF'/%3E%3Cstop offset='1' stop-color='%230A6FD4'/%3E%3C/linearGradient%3E%3ClinearGradient id='uf' x1='0' y1='0' x2='0' y2='1'%3E%3Cstop offset='0' stop-color='%230A84FF'/%3E%3Cstop offset='1' stop-color='%230066CC'/%3E%3C/linearGradient%3E%3C/defs%3E%3Ccircle cx='32' cy='32' r='30' fill='url(%23bg)'/%3E%3Ccircle cx='32' cy='32' r='29' fill='none' stroke='%23BDE0FE' stroke-width='.8'/%3E%3Cpath d='M14 56Q14 44 20 41L44 41Q50 44 50 56Z' fill='url(%23uf)'/%3E%3Cpath d='M28 41L28 48M36 41L36 48' stroke='rgba(255,255,255,.35)' stroke-width='1'/%3E%3Cpath d='M30 41L32 44L34 41' fill='none' stroke='white' stroke-width='1' stroke-linejoin='round'/%3E%3Ccircle cx='32' cy='30' r='15' fill='url(%23sk)'/%3E%3Cpath d='M17 27Q17 13 32 12Q47 13 47 27L47 24Q46 20 42 19L22 19Q18 20 17 24Z' fill='url(%23hr)'/%3E%3Cpath d='M17 27Q17 25 19 24L45 24Q47 25 47 27Q46 26 44 25.5L20 25.5Q18 26 17 27Z' fill='url(%23hr)' opacity='.6'/%3E%3Cpath d='M19 24L19 21.5Q19 17 25 16L39 16Q45 17 45 21.5L45 24Z' fill='url(%23cp)'/%3E%3Cpath d='M19 22L45 22' stroke='rgba(255,255,255,.3)' stroke-width='.7'/%3E%3Cellipse cx='32' cy='17.5' rx='3.5' ry='2' fill='url(%23cp)' stroke='%230A84FF' stroke-width='.3'/%3E%3Ccircle cx='32' cy='17.5' r='1.2' fill='%23C8102E'/%3E%3Cellipse cx='26' cy='31.5' rx='2.8' ry='3.2' fill='white'/%3E%3Cellipse cx='38' cy='31.5' rx='2.8' ry='3.2' fill='white'/%3E%3Cellipse cx='26.6' cy='31.8' rx='1.8' ry='2.2' fill='%232C1810'/%3E%3Cellipse cx='38.6' cy='31.8' rx='1.8' ry='2.2' fill='%232C1810'/%3E%3Ccircle cx='27.6' cy='30.6' r='.9' fill='white' opacity='.9'/%3E%3Ccircle cx='39.6' cy='30.6' r='.9' fill='white' opacity='.9'/%3E%3Cpath d='M22 29.5Q23 28.5 24 29' fill='none' stroke='%232C1810' stroke-width='.7' stroke-linecap='round'/%3E%3Cpath d='M40 29Q41 28.5 42 29.5' fill='none' stroke='%232C1810' stroke-width='.7' stroke-linecap='round'/%3E%3Cellipse cx='22.5' cy='35' rx='2.5' ry='1.5' fill='%23FFB5A7' opacity='.45'/%3E%3Cellipse cx='41.5' cy='35' rx='2.5' ry='1.5' fill='%23FFB5A7' opacity='.45'/%3E%3Cpath d='M29 37.2Q30.5 39 32 39Q33.5 39 35 37.2' fill='none' stroke='%23C0735A' stroke-width='1.2' stroke-linecap='round'/%3E%3C/svg%3E",
    imgSm:"data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='48' height='48' viewBox='0 0 64 64'%3E%3Cdefs%3E%3CradialGradient id='bg' cx='50%25' cy='45%25' r='50%25'%3E%3Cstop offset='0' stop-color='%23E8F4FD'/%3E%3Cstop offset='1' stop-color='%23D0E8FF'/%3E%3C/radialGradient%3E%3CradialGradient id='sk' cx='45%25' cy='38%25' r='55%25'%3E%3Cstop offset='0' stop-color='%23FFF0E6'/%3E%3Cstop offset='.6' stop-color='%23FFE0C9'/%3E%3Cstop offset='1' stop-color='%23F5CBA7'/%3E%3C/radialGradient%3E%3ClinearGradient id='hr' x1='0' y1='0' x2='0' y2='1'%3E%3Cstop offset='0' stop-color='%233D2B1F'/%3E%3Cstop offset='1' stop-color='%23241A12'/%3E%3C/linearGradient%3E%3ClinearGradient id='cp' x1='0' y1='0' x2='1' y2='1'%3E%3Cstop offset='0' stop-color='%231E90FF'/%3E%3Cstop offset='1' stop-color='%230A6FD4'/%3E%3C/linearGradient%3E%3ClinearGradient id='uf' x1='0' y1='0' x2='0' y2='1'%3E%3Cstop offset='0' stop-color='%230A84FF'/%3E%3Cstop offset='1' stop-color='%230066CC'/%3E%3C/linearGradient%3E%3C/defs%3E%3Ccircle cx='32' cy='32' r='30' fill='url(%23bg)'/%3E%3Ccircle cx='32' cy='32' r='29' fill='none' stroke='%23BDE0FE' stroke-width='.8'/%3E%3Cpath d='M14 56Q14 44 20 41L44 41Q50 44 50 56Z' fill='url(%23uf)'/%3E%3Cpath d='M28 41L28 48M36 41L36 48' stroke='rgba(255,255,255,.35)' stroke-width='1'/%3E%3Cpath d='M30 41L32 44L34 41' fill='none' stroke='white' stroke-width='1' stroke-linejoin='round'/%3E%3Ccircle cx='32' cy='30' r='15' fill='url(%23sk)'/%3E%3Cpath d='M17 27Q17 13 32 12Q47 13 47 27L47 24Q46 20 42 19L22 19Q18 20 17 24Z' fill='url(%23hr)'/%3E%3Cpath d='M17 27Q17 25 19 24L45 24Q47 25 47 27Q46 26 44 25.5L20 25.5Q18 26 17 27Z' fill='url(%23hr)' opacity='.6'/%3E%3Cpath d='M19 24L19 21.5Q19 17 25 16L39 16Q45 17 45 21.5L45 24Z' fill='url(%23cp)'/%3E%3Cellipse cx='26' cy='31.5' rx='2.8' ry='3.2' fill='white'/%3E%3Cellipse cx='38' cy='31.5' rx='2.8' ry='3.2' fill='white'/%3E%3Cellipse cx='26.6' cy='31.8' rx='1.8' ry='2.2' fill='%232C1810'/%3E%3Cellipse cx='38.6' cy='31.8' rx='1.8' ry='2.2' fill='%232C1810'/%3E%3Ccircle cx='27.6' cy='30.6' r='.9' fill='white' opacity='.9'/%3E%3Ccircle cx='39.6' cy='30.6' r='.9' fill='white' opacity='.9'/%3E%3Cellipse cx='22.5' cy='35' rx='2.5' ry='1.5' fill='%23FFB5A7' opacity='.45'/%3E%3Cellipse cx='41.5' cy='35' rx='2.5' ry='1.5' fill='%23FFB5A7' opacity='.45'/%3E%3Cpath d='M29 37.2Q30.5 39 32 39Q33.5 39 35 37.2' fill='none' stroke='%23C0735A' stroke-width='1.2' stroke-linecap='round'/%3E%3C/svg%3E",
    theme:{pri:'#0A84FF',priDk:'#0066CC',accent:'#1BFFFF',bg:'#F2F2F7',cardGrad:'linear-gradient(135deg,#2E3192,#1BFFFF)',fabRing:'#0A84FF',chatHd:'#0A84FF',greetEmoji:'✈️'},
    tone:'丁寧で温かいコンシェルジュ口調。「〜ですね！」「お任せください」のように親切で頼れる話し方。旅行の専門知識が豊富で、的確なアドバイスを提供する。',
    rpgImg:"data:image/svg+xml,%3Csvg xmlns=%27http://www.w3.org/2000/svg%27 width=%27400%27 height=%27520%27 viewBox=%278 8 48 52%27%3E%3Cdefs%3E%3CradialGradient id=%27sk%27 cx=%2745%25%27 cy=%2738%25%27 r=%2755%25%27%3E%3Cstop offset=%270%27 stop-color=%27%23FFF0E6%27/%3E%3Cstop offset=%27.6%27 stop-color=%27%23FFE0C9%27/%3E%3Cstop offset=%271%27 stop-color=%27%23F5CBA7%27/%3E%3C/radialGradient%3E%3ClinearGradient id=%27hr%27 x1=%270%27 y1=%270%27 x2=%270%27 y2=%271%27%3E%3Cstop offset=%270%27 stop-color=%27%233D2B1F%27/%3E%3Cstop offset=%271%27 stop-color=%27%23241A12%27/%3E%3C/linearGradient%3E%3ClinearGradient id=%27cp%27 x1=%270%27 y1=%270%27 x2=%271%27 y2=%271%27%3E%3Cstop offset=%270%27 stop-color=%27%231E90FF%27/%3E%3Cstop offset=%271%27 stop-color=%27%230A6FD4%27/%3E%3C/linearGradient%3E%3ClinearGradient id=%27uf%27 x1=%270%27 y1=%270%27 x2=%270%27 y2=%271%27%3E%3Cstop offset=%270%27 stop-color=%27%230A84FF%27/%3E%3Cstop offset=%271%27 stop-color=%27%230066CC%27/%3E%3C/linearGradient%3E%3C/defs%3E%3Cpath d=%27M14 56Q14 44 20 41L44 41Q50 44 50 56L50 62 14 62Z%27 fill=%27url(%23uf)%27/%3E%3Cpath d=%27M28 41L28 48M36 41L36 48%27 stroke=%27rgba(255,255,255,.35)%27 stroke-width=%271%27/%3E%3Cpath d=%27M30 41L32 44L34 41%27 fill=%27none%27 stroke=%27white%27 stroke-width=%271%27 stroke-linejoin=%27round%27/%3E%3Ccircle cx=%2732%27 cy=%2730%27 r=%2715%27 fill=%27url(%23sk)%27/%3E%3Cpath d=%27M17 27Q17 13 32 12Q47 13 47 27L47 24Q46 20 42 19L22 19Q18 20 17 24Z%27 fill=%27url(%23hr)%27/%3E%3Cpath d=%27M17 27Q17 25 19 24L45 24Q47 25 47 27Q46 26 44 25.5L20 25.5Q18 26 17 27Z%27 fill=%27url(%23hr)%27 opacity=%27.6%27/%3E%3Cpath d=%27M19 24L19 21.5Q19 17 25 16L39 16Q45 17 45 21.5L45 24Z%27 fill=%27url(%23cp)%27/%3E%3Cpath d=%27M19 22L45 22%27 stroke=%27rgba(255,255,255,.3)%27 stroke-width=%27.7%27/%3E%3Cellipse cx=%2732%27 cy=%2717.5%27 rx=%273.5%27 ry=%272%27 fill=%27url(%23cp)%27 stroke=%27%230A84FF%27 stroke-width=%27.3%27/%3E%3Ccircle cx=%2732%27 cy=%2717.5%27 r=%271.2%27 fill=%27%23C8102E%27/%3E%3Cellipse cx=%2726%27 cy=%2731.5%27 rx=%272.8%27 ry=%273.2%27 fill=%27white%27/%3E%3Cellipse cx=%2738%27 cy=%2731.5%27 rx=%272.8%27 ry=%273.2%27 fill=%27white%27/%3E%3Cellipse cx=%2726.6%27 cy=%2731.8%27 rx=%271.8%27 ry=%272.2%27 fill=%27%232C1810%27/%3E%3Cellipse cx=%2738.6%27 cy=%2731.8%27 rx=%271.8%27 ry=%272.2%27 fill=%27%232C1810%27/%3E%3Ccircle cx=%2727.6%27 cy=%2730.6%27 r=%27.9%27 fill=%27white%27 opacity=%27.9%27/%3E%3Ccircle cx=%2739.6%27 cy=%2730.6%27 r=%27.9%27 fill=%27white%27 opacity=%27.9%27/%3E%3Ccircle cx=%2725.8%27 cy=%2732.2%27 r=%27.4%27 fill=%27white%27 opacity=%27.6%27/%3E%3Ccircle cx=%2737.8%27 cy=%2732.2%27 r=%27.4%27 fill=%27white%27 opacity=%27.6%27/%3E%3Cpath d=%27M22 29.5Q23 28.5 24 29%27 fill=%27none%27 stroke=%27%232C1810%27 stroke-width=%27.7%27 stroke-linecap=%27round%27/%3E%3Cpath d=%27M40 29Q41 28.5 42 29.5%27 fill=%27none%27 stroke=%27%232C1810%27 stroke-width=%27.7%27 stroke-linecap=%27round%27/%3E%3Cellipse cx=%2722.5%27 cy=%2735%27 rx=%272.5%27 ry=%271.5%27 fill=%27%23FFB5A7%27 opacity=%27.45%27/%3E%3Cellipse cx=%2741.5%27 cy=%2735%27 rx=%272.5%27 ry=%271.5%27 fill=%27%23FFB5A7%27 opacity=%27.45%27/%3E%3Cpath d=%27M29 37.2Q30.5 39 32 39Q33.5 39 35 37.2%27 fill=%27none%27 stroke=%27%23C0735A%27 stroke-width=%271.2%27 stroke-linecap=%27round%27/%3E%3Cellipse cx=%2732%27 cy=%2737.5%27 rx=%271.8%27 ry=%27.6%27 fill=%27%23E8967A%27 opacity=%27.4%27/%3E%3C/svg%3E",
    greet:'こんにちは！案内人のつむぎです。日本の旅を一緒に楽しみましょう！'
  }
];
const MOODS={
  normal:{emoji:'',label:'通常',halo:'transparent',badge:''},
  happy:{emoji:'✨',label:'うれしい',halo:'rgba(52,199,89,.25)',badge:'b-grn'},
  thinking:{emoji:'💭',label:'考え中',halo:'rgba(10,132,255,.2)',badge:'b-blu'},
  alert:{emoji:'⚠️',label:'注意',halo:'rgba(255,149,0,.25)',badge:'b-org'},
  cheer:{emoji:'💪',label:'応援',halo:'rgba(10,132,255,.15)',badge:'b-blu'}
};
function getSelectedAvatar(){
  const id=getAdminSetting('avatar','tsumugi');
  return AVATARS.find(a=>a.id===id)||AVATARS.find(a=>a.id==='tsumugi')||AVATARS[AVATARS.length-1];
}
function setSelectedAvatar(id){
  setAdminSetting('avatar',id);
  applyAvatarTheme();
  updateAvatarUI();
}
function applyAvatarTheme(){
  const av=getSelectedAvatar();
  const t=av.theme;
  const r=document.documentElement.style;
  r.setProperty('--pri',t.pri);
  r.setProperty('--pri-dk',t.priDk);
  r.setProperty('--ic',t.cardGrad);
}
let _currentMood='normal';
function setAvatarMood(mood){
  _currentMood=mood||'normal';
  updateAvatarUI();
}
function updateAvatarUI(){
  const av=getSelectedAvatar();
  const mood=MOODS[_currentMood]||MOODS.normal;
  /* FAB */
  const fab=$('chatFab');
  if(fab){
    fab.style.borderColor=av.theme.fabRing;
    fab.style.boxShadow='0 8px 24px '+av.theme.fabRing+'55';
    const fabImg=fab.querySelector('.fab-avatar');
    if(fabImg) fabImg.src=av.imgSm;
    const moodBadge=fab.querySelector('.fab-mood');
    if(moodBadge){
      moodBadge.textContent=mood.emoji;
      moodBadge.style.display=mood.emoji?'flex':'none';
    }
    fab.style.background=mood.halo!=='transparent'?mood.halo:'#fff';
  }
  /* Chat header */
  const chatAvImg=$('chatAvatarImg');
  if(chatAvImg) chatAvImg.src=av.imgSm;
  const chatAvName=$('chatAvatarName');
  if(chatAvName) chatAvName.textContent=av.name;
}

/* ── Read API keys from localStorage (replacing hardcoded values) ── */
function getGoogleMapsEmbedApiKey(){ return getAdminSetting('googleMapsApiKey',''); }
function getOpenWeatherApiKey(){ return ''; /* no longer hardcoded */ }
const PLACES_PROVIDER = 'overpass';
const config = { DEFAULT_LOCATION: { lat: 35.6812, lon: 139.7671, name: '東京駅' } };

const I={
  back:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M15 18l-6-6 6-6"/></svg>',
  chev:'<svg class="chev" width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M9 18l6-6-6-6"/></svg>',
  card:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="5" width="20" height="14" rx="2"/><path d="M2 10h20"/></svg>',
  route:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M9 18l6-6-6-6"/></svg>',
  bag:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="4" y="4" width="16" height="16" rx="2"/><path d="M4 10h16M10 4v16"/></svg>',
  tour:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><path d="M12 8v8M8 12h8"/></svg>',
  sos:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0zM12 9v4M12 17h.01"/></svg>',
  yen:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>',
  plane:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M21.94 10.63l-2.88-5a2.05 2.05 0 0 0-2.81-.7l-3.32 1.91-6.19-2.3-1.68 1.68 4.31 4.54-3.5 2-2.19-.84-1.39 1.39 3.86 1.84 1.84 3.86 1.39-1.39-.84-2.19 2-3.5 4.54 4.31 1.68-1.68-2.3-6.19 1.91-3.32a2.05 2.05 0 0 0-.7-2.81z"/></svg>',
  plus:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>',
  pin:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>',
  loc:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="3"/></svg>',
  clock:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>',
  cal:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="3" y="4" width="18" height="18" rx="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>',
  lock:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="3" y="11" width="18" height="11" rx="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg>',
  flag:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M4 15s1-1 4-1 5 2 8 2 4-1 4-1V3s-1 1-4 1-5-2-8-2-4 1-4 1zM4 22v-7"/></svg>',
  bolt:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"/></svg>',
  send:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 2L11 13M22 2l-7 20-4-9-9-4 20-7z"/></svg>',
  search:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="11" cy="11" r="8"/><line x1="21" y1="21" x2="16.65" y2="16.65"/></svg>',
  health:'<svg width="20" height="20" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 12h-4l-3 9L9 3l-3 9H2"/></svg>',
  shield:'<svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>',
  phone:'<svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72c.13.876.37 1.735.7 2.56a2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45c.825.33 1.684.57 2.56.7A2 2 0 0 1 22 16.92z"/></svg>',
  home:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/></svg>',
  check:'<svg width="40" height="40" fill="none" stroke="currentColor" stroke-width="3" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>',
  star:'<svg width="12" height="12" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>',
  arrow:'<svg width="24" height="24" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M5 12h14M12 5l7 7-7 7"/></svg>',
  info:'<svg width="14" height="14" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>',
  gear:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-4 0v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1 0-4h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 4 0v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 0 4h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>',
  ext:'<svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>',
  ticket:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M3 7v4a2 2 0 0 1 0 4v4a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-4a2 2 0 0 1 0-4V7a2 2 0 0 0-2-2H5a2 2 0 0 0-2 2zM13 5v2M13 11v2M13 17v2"/></svg>',
  list:'<svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><line x1="8" y1="6" x2="21" y2="6"/><line x1="8" y1="12" x2="21" y2="12"/><line x1="8" y1="18" x2="21" y2="18"/><line x1="3" y1="6" x2="3.01" y2="6"/><line x1="3" y1="12" x2="3.01" y2="12"/><line x1="3" y1="18" x2="3.01" y2="18"/></svg>'
};

function charaSVG(size){
  const s = size||44;
  const uid = 'ts'+s+Math.random().toString(36).slice(2,6);
  return `<svg width="${s}" height="${s}" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" style="display:block">
    <defs>
      <radialGradient id="bg${uid}" cx="50%" cy="45%" r="50%"><stop offset="0%" stop-color="#E8F4FD"/><stop offset="100%" stop-color="#D0E8FF"/></radialGradient>
      <radialGradient id="sk${uid}" cx="45%" cy="38%" r="55%"><stop offset="0%" stop-color="#FFF0E6"/><stop offset="60%" stop-color="#FFE0C9"/><stop offset="100%" stop-color="#F5CBA7"/></radialGradient>
      <linearGradient id="hr${uid}" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#3D2B1F"/><stop offset="100%" stop-color="#241A12"/></linearGradient>
      <linearGradient id="cp${uid}" x1="0" y1="0" x2="1" y2="1"><stop offset="0%" stop-color="#1E90FF"/><stop offset="100%" stop-color="#0A6FD4"/></linearGradient>
      <linearGradient id="uf${uid}" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#0A84FF"/><stop offset="100%" stop-color="#0066CC"/></linearGradient>
    </defs>
    <circle cx="32" cy="32" r="30" fill="url(#bg${uid})"/>
    <circle cx="32" cy="32" r="29" fill="none" stroke="#BDE0FE" stroke-width=".8"/>
    <path d="M14 56 Q14 44 20 41 L44 41 Q50 44 50 56 Z" fill="url(#uf${uid})"/>
    <path d="M28 41 L28 48 M36 41 L36 48" stroke="rgba(255,255,255,.35)" stroke-width="1"/>
    <path d="M30 41 L32 44 L34 41" fill="none" stroke="#FFF" stroke-width="1" stroke-linejoin="round"/>
    <circle cx="32" cy="30" r="15" fill="url(#sk${uid})"/>
    <path d="M17 27 Q17 13 32 12 Q47 13 47 27 L47 24 Q46 20 42 19 L22 19 Q18 20 17 24 Z" fill="url(#hr${uid})"/>
    <path d="M17 27 Q17 25 19 24 L45 24 Q47 25 47 27 Q46 26 44 25.5 L20 25.5 Q18 26 17 27 Z" fill="url(#hr${uid})" opacity=".6"/>
    <path d="M19 24 L19 21.5 Q19 17 25 16 L39 16 Q45 17 45 21.5 L45 24 Z" fill="url(#cp${uid})"/>
    <path d="M19 22 L45 22" stroke="rgba(255,255,255,.3)" stroke-width=".7"/>
    <ellipse cx="32" cy="17.5" rx="3.5" ry="2" fill="url(#cp${uid})" stroke="#0A84FF" stroke-width=".3"/>
    <circle cx="32" cy="17.5" r="1.2" fill="#C8102E"/>
    <ellipse cx="26" cy="31.5" rx="2.8" ry="3.2" fill="#FFF"/>
    <ellipse cx="38" cy="31.5" rx="2.8" ry="3.2" fill="#FFF"/>
    <ellipse cx="26.6" cy="31.8" rx="1.8" ry="2.2" fill="#2C1810"/>
    <ellipse cx="38.6" cy="31.8" rx="1.8" ry="2.2" fill="#2C1810"/>
    <circle cx="27.6" cy="30.6" r=".9" fill="#FFF" opacity=".9"/>
    <circle cx="39.6" cy="30.6" r=".9" fill="#FFF" opacity=".9"/>
    <circle cx="25.8" cy="32.2" r=".4" fill="#FFF" opacity=".6"/>
    <circle cx="37.8" cy="32.2" r=".4" fill="#FFF" opacity=".6"/>
    <path d="M22 29.5 Q23 28.5 24 29" fill="none" stroke="#2C1810" stroke-width=".7" stroke-linecap="round"/>
    <path d="M40 29 Q41 28.5 42 29.5" fill="none" stroke="#2C1810" stroke-width=".7" stroke-linecap="round"/>
    <ellipse cx="22.5" cy="35" rx="2.5" ry="1.5" fill="#FFB5A7" opacity=".45"/>
    <ellipse cx="41.5" cy="35" rx="2.5" ry="1.5" fill="#FFB5A7" opacity=".45"/>
    <path d="M29 37.2 Q30.5 39 32 39 Q33.5 39 35 37.2" fill="none" stroke="#C0735A" stroke-width="1.2" stroke-linecap="round"/>
    <ellipse cx="32" cy="37.5" rx="1.8" ry=".6" fill="#E8967A" opacity=".4"/>
  </svg>`;
}

const $=s=>document.getElementById(s);
const $$=s=>document.querySelectorAll(s);
const helpers = {
  esc(s){ const d=document.createElement('div'); d.textContent=s==null?'':String(s); return d.innerHTML; },
  sh(backId,title){ return `<div class="sh"><button class="back" onclick="nav('${helpers.esc(backId)}')">${I.back}</button><h2>${helpers.esc(title)}</h2></div>`; },
  toast(m){ const t=$('toast'); t.textContent=m; t.classList.add('show'); setTimeout(()=>t.classList.remove('show'),2500); },
  haversineKm(a,b){
    const R=6371, toRad=d=>d*Math.PI/180;
    const dLat=toRad(b.lat-a.lat), dLon=toRad(b.lon-a.lon);
    const s=Math.sin(dLat/2)**2+Math.cos(toRad(a.lat))*Math.cos(toRad(b.lat))*Math.sin(dLon/2)**2;
    return R*2*Math.atan2(Math.sqrt(s),Math.sqrt(1-s));
  },
  formatDistance(km){ if(km==null||isNaN(km)) return ''; return km<1 ? Math.round(km*1000)+'m' : km.toFixed(1)+'km'; },
  getClothingAdvice(temp, code){
    let o='';
    if(temp<=5) o='厚手のコート+防寒小物がおすすめ';
    else if(temp<=11) o='コートまたはダウンがおすすめ';
    else if(temp<=16) o='薄手のジャケットやカーディガン';
    else if(temp<=22) o='長袖または軽い羽織りが快適';
    else if(temp<=27) o='半袖中心で快適に過ごせます';
    else o='かなり暑いので涼しい服装・水分補給を';
    if([51,53,55,61,63,65,80,81,82,95,96,99].includes(code)) o+=' / ☂傘を忘れずに';
    return o;
  },
  mapWeatherToIcon(code){
    if(code===0) return {em:'☀️',cls:'sunny',label:'晴れ'};
    if(code<=3) return {em:'⛅',cls:'',label:'曇り'};
    if(code<=48) return {em:'🌫️',cls:'',label:'霧'};
    if(code<=67) return {em:'🌧️',cls:'rainy',label:'雨'};
    if(code<=77) return {em:'❄️',cls:'snow',label:'雪'};
    if(code<=82) return {em:'🌦️',cls:'rainy',label:'にわか雨'};
    return {em:'⛈️',cls:'rainy',label:'雷雨'};
  },
  fmtDate(d){ return `${d.getMonth()+1}/${d.getDate()}`; },
  dayLabel(d){ return ['日','月','火','水','木','金','土'][d.getDay()]; },
  todayISO(){ return new Date().toISOString().split('T')[0]; }
};

const state = {
  session:{ isLoggedIn:false, email:'' },
  profile:null,
  location:{ permission:'unset', coords:null, label:'', fallback:'東京' },
  weather:null, weatherForecast:null,
  nearbySpots:[], selectedSpot:null,
  mobility:{ origin:'', destination:'', category:'public', mode:'train' },
  balance:4500, chargeAmt:3000,
  currentView:'home', weatherDetailTab:'today',
  completedTodos:{}, selectedTodo:null,
  ticket:{ selectedId:null, date: helpers.todayISO(), adult:1, child:0, highlight:null },
  adminTab:'main',
  tourSelections:{ themes:[], energy:'normal', crowd:'ok', time:'half', freeText:'' },
  generatedTourPlans:null,
  selectedTourPlan:null
};
const STATE_KEY='assisTripStateV3';
function saveState(){
  try{
    const {profile,location,session,mobility,completedTodos}=state;
    localStorage.setItem(STATE_KEY, JSON.stringify({profile,location,session,mobility,completedTodos}));
  }catch(e){}
}
function loadState(){
  try{
    const d=localStorage.getItem(STATE_KEY); if(!d) return;
    const p=JSON.parse(d);
    Object.assign(state.session,p.session||{});
    if(p.profile) state.profile=p.profile;
    Object.assign(state.location,p.location||{});
    Object.assign(state.mobility,p.mobility||{});
    state.completedTodos = p.completedTodos || {};
  }catch(e){}
}
const PROFILE_OPTS = {
  nationality:['日本','中国','韓国','アメリカ','イギリス','フランス','ドイツ','オーストラリア','タイ','その他'],
  languages:['日本語','English','中文','한국어','Français','Español','Deutsch'],
  gender:['男性','女性','その他','回答しない'],
  preferences:['グルメ','買い物','歴史','アート','自然','静かな場所','アニメ・ポップカルチャー','温泉'],
  japanVisitCount:['初めて','2〜3回','4回以上'],
  cities:['東京','大阪','京都','福岡','札幌','名古屋','横浜','沖縄']
};
const CITY_COORDS = {
  '東京':{lat:35.6812,lon:139.7671}, '大阪':{lat:34.6937,lon:135.5023}, '京都':{lat:35.0116,lon:135.7681},
  '福岡':{lat:33.5902,lon:130.4017}, '札幌':{lat:43.0621,lon:141.3544}, '名古屋':{lat:35.1815,lon:136.9066},
  '横浜':{lat:35.4437,lon:139.638}, '沖縄':{lat:26.2124,lon:127.6792}
};

const CITY_SPOTS = {
  '東京':[
    {name:'浅草寺',category:'寺院',emoji:'🏯',lat:35.7148,lon:139.7967,desc:'雷門で名高い東京屈指の古刹。仲見世通りの散策も楽しめます。'},
    {name:'東京国立博物館',category:'美術館/博物館',emoji:'🖼️',lat:35.7188,lon:139.7766,desc:'日本最古の博物館。日本美術・工芸の名品が集まります。'},
    {name:'上野恩賜公園',category:'公園',emoji:'🌸',lat:35.7156,lon:139.7730,desc:'美術館・動物園が集まる都心の大公園。桜の名所。'},
    {name:'丸の内仲通り',category:'ショッピング',emoji:'🛍️',lat:35.6795,lon:139.7644,desc:'洗練された並木道。ブランドショップとカフェが並びます。'},
    {name:'明治神宮',category:'神社',emoji:'⛩️',lat:35.6764,lon:139.6993,desc:'原宿に広がる緑豊かな神宮。静かな参道が特徴。'},
    {name:'東京スカイツリー',category:'展望',emoji:'🌆',lat:35.7101,lon:139.8107,desc:'高さ634mの展望タワー。東京全体を一望できます。'}
  ],
  '大阪':[
    {name:'大阪城',category:'城',emoji:'🏯',lat:34.6873,lon:135.5262,desc:'大阪のシンボル。天守閣からの眺めと歴史展示。'},
    {name:'道頓堀',category:'ショッピング',emoji:'🛍️',lat:34.6687,lon:135.5023,desc:'グリコサインで有名な繁華街。食い倒れの街。'},
    {name:'通天閣',category:'展望',emoji:'🌆',lat:34.6525,lon:135.5063,desc:'新世界エリアの展望タワー。下町情緒を感じる。'},
    {name:'住吉大社',category:'神社',emoji:'⛩️',lat:34.6125,lon:135.4931,desc:'全国の住吉神社の総本社。太鼓橋が美しい。'},
    {name:'海遊館',category:'水族館',emoji:'🐟',lat:34.6547,lon:135.4289,desc:'世界最大級の水族館。ジンベエザメも見られます。'}
  ],
  '京都':[
    {name:'清水寺',category:'寺院',emoji:'🏯',lat:34.9949,lon:135.7850,desc:'京都屈指の名刹。清水の舞台からの眺めは絶景。'},
    {name:'伏見稲荷大社',category:'神社',emoji:'⛩️',lat:34.9671,lon:135.7727,desc:'千本鳥居で世界的に有名な稲荷信仰の総本宮。'},
    {name:'金閣寺',category:'寺院',emoji:'🏯',lat:35.0394,lon:135.7292,desc:'金箔で覆われた楼閣。池に映る姿が美しい。'},
    {name:'嵐山 渡月橋',category:'景勝',emoji:'🌉',lat:35.0129,lon:135.6771,desc:'桂川にかかる象徴的な橋。竹林の小径も近く。'},
    {name:'祇園 花見小路',category:'ショッピング',emoji:'🏮',lat:35.0036,lon:135.7750,desc:'京都らしい町並み。夕方からは舞妓さんの姿も。'}
  ],
  '福岡':[
    {name:'太宰府天満宮',category:'神社',emoji:'⛩️',lat:33.5213,lon:130.5348,desc:'学問の神様・菅原道真公を祀る。梅の名所。'},
    {name:'中洲屋台',category:'グルメ',emoji:'🍜',lat:33.5920,lon:130.4061,desc:'福岡名物の屋台街。ラーメンや焼き鳥を楽しめます。'},
    {name:'博多駅',category:'ショッピング',emoji:'🛍️',lat:33.5901,lon:130.4206,desc:'九州最大級の駅ビル。お土産探しにも最適。'}
  ],
  '札幌':[
    {name:'札幌時計台',category:'史跡',emoji:'🕰️',lat:43.0629,lon:141.3537,desc:'札幌のシンボル。明治時代の貴重な建築。'},
    {name:'大通公園',category:'公園',emoji:'🌳',lat:43.0603,lon:141.3545,desc:'札幌中心部を東西に貫く市民公園。'},
    {name:'札幌場外市場',category:'グルメ',emoji:'🦀',lat:43.0797,lon:141.3353,desc:'北海道の新鮮な海産物が集まる市場。'}
  ],
  '名古屋':[
    {name:'名古屋城',category:'城',emoji:'🏯',lat:35.1856,lon:136.8997,desc:'金のシャチホコで知られる徳川の名城。'},
    {name:'熱田神宮',category:'神社',emoji:'⛩️',lat:35.1281,lon:136.9086,desc:'三種の神器の一つ草薙剣を祀る古社。'},
    {name:'大須商店街',category:'ショッピング',emoji:'🛍️',lat:35.1605,lon:136.8999,desc:'下町情緒とサブカルが混ざり合う活気ある商店街。'}
  ],
  '横浜':[
    {name:'横浜赤レンガ倉庫',category:'ショッピング',emoji:'🛍️',lat:35.4529,lon:139.6425,desc:'歴史ある倉庫を改装した商業施設。海辺の景色も楽しめます。'},
    {name:'山下公園',category:'公園',emoji:'🌊',lat:35.4445,lon:139.6497,desc:'港の景観が美しい横浜の定番公園。'},
    {name:'横浜中華街',category:'グルメ',emoji:'🥟',lat:35.4436,lon:139.6463,desc:'日本最大の中華街。点心や中華料理が楽しめます。'}
  ],
  '沖縄':[
    {name:'首里城公園',category:'城',emoji:'🏯',lat:26.2173,lon:127.7188,desc:'琉球王国の王城跡。独特の赤瓦が印象的。'},
    {name:'国際通り',category:'ショッピング',emoji:'🛍️',lat:26.2145,lon:127.6877,desc:'那覇最大の繁華街。お土産やグルメが揃います。'},
    {name:'美ら海水族館',category:'水族館',emoji:'🐠',lat:26.6944,lon:127.8777,desc:'世界最大級の水槽でジンベエザメが泳ぐ水族館。'}
  ]
};
function getCityKeyFromCoords(lat,lon){
  let best=null, min=9999;
  for(const k in CITY_COORDS){
    const c=CITY_COORDS[k];
    const d=helpers.haversineKm({lat,lon},{lat:c.lat,lon:c.lon});
    if(d<min){ min=d; best=k; }
  }
  return best;
}

const services = {
  getCurrentLocation(){
    return new Promise(resolve=>{
      if(!navigator.geolocation){ resolve(null); return; }
      navigator.geolocation.getCurrentPosition(
        pos=>resolve({lat:pos.coords.latitude,lon:pos.coords.longitude}),
        ()=>resolve(null),
        {timeout:8000,maximumAge:300000}
      );
    });
  },
  resolveCoords(){
    const L=state.location;
    if(L.permission==='granted' && L.coords) return {...L.coords,label:L.label||'現在地'};
    const c=CITY_COORDS[L.fallback];
    if(c) return {...c,label:L.fallback};
    return {...config.DEFAULT_LOCATION,label:config.DEFAULT_LOCATION.name};
  },
  async fetchWeather(lat,lon){
    const owKey = getOpenWeatherApiKey();
    if(owKey){
      try{
        const cur = await fetch(`https://api.openweathermap.org/data/2.5/weather?lat=${lat}&lon=${lon}&units=metric&lang=ja&appid=${owKey}`).then(r=>r.json());
        const fc  = await fetch(`https://api.openweathermap.org/data/2.5/forecast?lat=${lat}&lon=${lon}&units=metric&lang=ja&appid=${owKey}`).then(r=>r.json());
        return services._fromOWM(cur,fc);
      }catch(e){ console.error('[OpenWeather] failed',e); }
    }
    return services._fetchOpenMeteo(lat,lon);
  },
  async _fetchOpenMeteo(lat,lon){
    try{
      const url = `https://api.open-meteo.com/v1/forecast?latitude=${lat}&longitude=${lon}`
        + `&current=temperature_2m,weather_code,relative_humidity_2m,wind_speed_10m`
        + `&hourly=temperature_2m,weather_code&forecast_hours=24`
        + `&daily=temperature_2m_max,temperature_2m_min,weather_code&forecast_days=7`
        + `&timezone=auto`;
      const d=await fetch(url).then(r=>r.json());
      const cur={
        temp:Math.round(d.current.temperature_2m),
        code:d.current.weather_code,
        tempMax:d.daily?.temperature_2m_max?.[0]!=null?Math.round(d.daily.temperature_2m_max[0]):null,
        tempMin:d.daily?.temperature_2m_min?.[0]!=null?Math.round(d.daily.temperature_2m_min[0]):null,
        humidity:d.current.relative_humidity_2m,
        wind:d.current.wind_speed_10m
      };
      const hourly=(d.hourly?.time||[]).slice(0,12).map((t,i)=>({
        time:new Date(t), temp:Math.round(d.hourly.temperature_2m[i]), code:d.hourly.weather_code[i]
      }));
      const daily=(d.daily?.time||[]).map((t,i)=>({
        date:new Date(t),
        max:Math.round(d.daily.temperature_2m_max[i]),
        min:Math.round(d.daily.temperature_2m_min[i]),
        code:d.daily.weather_code[i]
      }));
      return { current:cur, hourly, daily };
    }catch(e){ console.error('[Open-Meteo] failed',e); return null; }
  },
  _fromOWM(cur,fc){
    const c = { temp:Math.round(cur.main.temp), code:services._owmToCode(cur.weather[0].id),
      tempMax:Math.round(cur.main.temp_max), tempMin:Math.round(cur.main.temp_min),
      humidity:cur.main.humidity, wind:cur.wind.speed };
    const hourly=(fc.list||[]).slice(0,12).map(x=>({ time:new Date(x.dt*1000), temp:Math.round(x.main.temp), code:services._owmToCode(x.weather[0].id) }));
    const byDay={};
    (fc.list||[]).forEach(x=>{
      const d=new Date(x.dt*1000); const k=d.toDateString();
      if(!byDay[k]) byDay[k]={date:d,min:x.main.temp_min,max:x.main.temp_max,code:services._owmToCode(x.weather[0].id)};
      else{ byDay[k].min=Math.min(byDay[k].min,x.main.temp_min); byDay[k].max=Math.max(byDay[k].max,x.main.temp_max); }
    });
    const daily=Object.values(byDay).slice(0,7).map(x=>({date:x.date,min:Math.round(x.min),max:Math.round(x.max),code:x.code}));
    return { current:c, hourly, daily };
  },
  _owmToCode(id){
    if(id>=200&&id<300) return 95; if(id>=300&&id<400) return 61;
    if(id>=500&&id<600) return id<502?61:(id<504?63:65);
    if(id>=600&&id<700) return 73; if(id>=700&&id<800) return 45;
    if(id===800) return 0; if(id===801) return 1; if(id===802) return 2; if(id>=803) return 3;
    return 3;
  },
  async fetchNearbySpots(lat,lon,radiusM=1500){
    const cityKey=getCityKeyFromCoords(lat,lon);
    const seed=(CITY_SPOTS[cityKey]||[]).map(s=>({
      ...s, distanceKm: helpers.haversineKm({lat,lon},{lat:s.lat,lon:s.lon}),
      website:'', opening:''
    }));
    const query=`[out:json][timeout:8];(
      node(around:${radiusM},${lat},${lon})[tourism~"^(museum|attraction|viewpoint|gallery|zoo|aquarium)$"][name];
      node(around:${radiusM},${lat},${lon})[historic~"^(shrine|temple|monument|castle)$"][name];
      node(around:${radiusM},${lat},${lon})[leisure~"^(park|garden)$"][name];
    );out center 20;`;
    let overpass=[];
    try{
      const r=await fetch('https://overpass-api.de/api/interpreter',{
        method:'POST',
        headers:{'Content-Type':'application/x-www-form-urlencoded'},
        body:'data='+encodeURIComponent(query)
      });
      const d=await r.json();
      overpass=(d.elements||[])
        .filter(e=>e.tags && (e.tags['name:ja']||e.tags.name))
        .map(e=>{
          const nm=e.tags['name:ja']||e.tags.name;
          if(nm.length<=2) return null;
          if(/^(公園|広場|カフェ|駅)$/.test(nm)) return null;
          const cat=services._classifySpot(e.tags);
          return {
            name:nm, category:cat.label, emoji:cat.emoji,
            lat:e.lat, lon:e.lon, distanceKm:helpers.haversineKm({lat,lon},{lat:e.lat,lon:e.lon}),
            website:e.tags.website||e.tags['contact:website']||'',
            opening:e.tags.opening_hours||'',
            desc: services._descForCat(cat.label, nm)
          };
        }).filter(Boolean);
    }catch(e){}
    const byName=new Map();
    seed.forEach(s=>byName.set(s.name,s));
    overpass.forEach(s=>{ if(!byName.has(s.name)) byName.set(s.name,s); });
    return Array.from(byName.values()).sort((a,b)=>a.distanceKm-b.distanceKm).slice(0,8);
  },
  _classifySpot(t){
    if(t.historic==='shrine') return {label:'神社',emoji:'⛩️'};
    if(t.historic==='temple') return {label:'寺院',emoji:'🏯'};
    if(t.historic==='castle') return {label:'城',emoji:'🏯'};
    if(t.historic) return {label:'史跡',emoji:'🏛️'};
    if(t.tourism==='museum'||t.tourism==='gallery') return {label:'美術館/博物館',emoji:'🖼️'};
    if(t.tourism==='viewpoint') return {label:'展望',emoji:'🌆'};
    if(t.tourism==='aquarium') return {label:'水族館',emoji:'🐟'};
    if(t.tourism==='zoo') return {label:'動物園',emoji:'🦁'};
    if(t.leisure==='park') return {label:'公園',emoji:'🌳'};
    if(t.leisure==='garden') return {label:'庭園',emoji:'🌸'};
    return {label:'スポット',emoji:'📍'};
  },
  _descForCat(c,n){
    const m={'神社':`${n}は近くの神社。落ち着いた時間を過ごせます。`,'寺院':`${n}は歴史ある寺院。日本文化を感じられます。`,'城':`${n}。歴史ある城址を見学できます。`,'美術館/博物館':`${n}でアート・展示に触れられます。`,'公園':`${n}は散策や休憩に好適なスポット。`,'庭園':`${n}は日本庭園の美を感じられる場所。`,'展望':`${n}は街を見渡せる展望スポット。`};
    return m[c] || `${n}は近くの注目スポットです。`;
  }
};

const MODE_GROUPS = [
  {k:'public', l:'公共交通機関', subs:[
    {k:'train', l:'電車', em:'🚃'},
    {k:'shinkansen', l:'新幹線', em:'🚅'},
    {k:'bus', l:'バス', em:'🚌'},
    {k:'flight', l:'飛行機', em:'✈️'}
  ]},
  {k:'private', l:'その他', subs:[
    {k:'taxi', l:'タクシー', em:'🚕'},
    {k:'car_hw', l:'自家用車(高速あり)', em:'🚗'},
    {k:'car_nohw', l:'自家用車(高速なし)', em:'🚙'},
    {k:'bicycle', l:'自転車', em:'🚲'}
  ]}
];
function modeToGoogle(m){
  switch(m){
    case 'train': case 'bus': case 'shinkansen': return {mode:'transit', avoid:''};
    case 'flight': return {mode:'flying', avoid:''};
    case 'taxi': case 'car_hw': return {mode:'driving', avoid:''};
    case 'car_nohw': return {mode:'driving', avoid:'highways'};
    case 'bicycle': return {mode:'bicycling', avoid:''};
    default: return {mode:'transit', avoid:''};
  }
}
function findModeMeta(k){
  for(const g of MODE_GROUPS){ const f=g.subs.find(s=>s.k===k); if(f) return f; }
  return {k, l:k, em:'🚃'};
}
function buildMapsEmbedURL(origin, destination, modeKey){
  const apiKey = getGoogleMapsEmbedApiKey();
  if(!apiKey) return null;
  if(!destination) return null;
  const g = modeToGoogle(modeKey);
  const p = new URLSearchParams({
    key: apiKey,
    origin: origin || '',
    destination: destination,
    mode: g.mode
  });
  if(g.avoid) p.set('avoid', g.avoid);
  return 'https://www.google.com/maps/embed/v1/directions?' + p.toString();
}
function buildMapsExternalURL(origin, destination, modeKey){
  const g = modeToGoogle(modeKey);
  const p = new URLSearchParams({ api:'1', destination: destination||'', travelmode:g.mode });
  if(origin) p.set('origin', origin);
  if(g.avoid) p.set('avoid', g.avoid);
  return 'https://www.google.com/maps/dir/?' + p.toString();
}
function openExt(url){ if(url) window.open(url,'_blank','noopener,noreferrer'); }

const TODO_DEFS = [
  {
    id:'refund', icon:'🧾', title:'免税の未確認事項があります',
    desc:'購入した免税品と書類を確認し、出国前に整理しましょう。',
    link:{label:'免税リファンド画面を開く', view:'refund'},
    items:['購入した免税品がすべて手元にある','レシート・免税購入記録票が揃っている','パスポートを携帯している','未確認の購入を「準備OK」にしている']
  },
  {
    id:'oac', icon:'🛂', title:'OACの可否確認が未完了です',
    desc:'空港外チェックイン(OAC)が使えるか事前に確認しましょう。',
    link:{label:'OAC画面を開く', view:'oac'},
    items:['フライト情報（便名・出発時刻）が分かっている','パスポート・予約番号を準備した','OACの利用可否を確認した','荷物の預け方（個数・サイズ）を確認した']
  },
  {
    id:'docs', icon:'📄', title:'出発前の必要書類を確認してください',
    desc:'パスポートやビザ、保険証書などを出発前に再確認しましょう。',
    items:['パスポートの有効期限','ビザ・在留カード（該当者）','航空券・eチケット','海外旅行保険の証書','帰国後に必要な書類（税関申告等）']
  },
  {
    id:'ic', icon:'💳', title:'交通系IC残高を確認してください',
    desc:'移動前にICカード残高の確認とチャージをしておきましょう。',
    link:{label:'チャージ画面を開く', view:'charge'},
    items:['現在のIC残高を確認した','必要に応じてチャージした','モバイルICが有効になっている']
  }
];
function visibleTodos(){ return TODO_DEFS.filter(t=>!state.completedTodos[t.id]); }

const menuItems=[
  {id:'home',icon:'home',label:'ホーム'},
  {id:'pay-top',icon:'card',label:'交通・決済'},
  {id:'mobility-hub',icon:'route',label:'経路・チケット'},
  {id:'baggage',icon:'bag',label:'手荷物配送',children:[
    {id:'baggage',label:'新しく予約する',ic:'plus'},
    {id:'history-baggage',label:'予約履歴',ic:'list'}
  ]},
  {id:'tour',icon:'tour',label:'観光ガイド',children:[
    {id:'tour',label:'新しくプランを作成',ic:'plus'},
    {id:'history-tours',label:'保存した旅行プラン',ic:'list'}
  ]},
  {id:'trouble',icon:'sos',label:'トラブル・SOS'},
  {id:'refund',icon:'yen',label:'免税リファンド'},
  {id:'oac',icon:'plane',label:'空港チェックイン (OAC)'},
  {id:'history-hub',icon:'list',label:'利用履歴'},
  {id:'settings',icon:'gear',label:'設定'}
];
const CUR_MAP = {
  'mobility':'mobility-hub','ticket':'mobility-hub','ticket-confirm':'mobility-hub','ticket-complete':'mobility-hub',
  'bag-form':'baggage','bag-confirm':'baggage','bag-complete':'baggage',
  'tour-results':'tour','tour-detail':'tour',
  'trouble-detail':'trouble',
  'refund-form':'refund','refund-confirm':'refund','refund-complete':'refund',
  'oac-form':'oac','oac-confirm':'oac','oac-complete':'oac',
  'charge':'pay-top','tap':'pay-top','ic-manage':'pay-top',
  'todo-detail':'home','admin-settings':'home',
  'history-tours':'history-hub','history-tour-detail':'history-hub',
  'history-baggage':'history-hub','history-baggage-detail':'history-hub',
  'history-tickets':'history-hub','history-refunds':'history-hub','history-oac':'history-hub'
};
const _menuExpanded={};
function nav(id){
  $$('.view').forEach(v=>v.classList.remove('active'));
  const el=$('v-'+id);
  if(el){el.classList.add('active');state.currentView=id}
  /* Render history views on demand */
  const histRenders={'history-hub':renderHistoryHub,'history-tours':renderHistoryTours,'history-baggage':renderHistoryBaggage,'history-tickets':renderHistoryTickets,'history-refunds':renderHistoryRefunds,'history-oac':renderHistoryOac};
  if(histRenders[id]) histRenders[id]();
  closeMenu(); buildMenu();
  document.body.classList.toggle('no-header', id==='login');
  updateAdminUI();
  window.scrollTo(0,0);
}
function openMenu(){$('sideMenu').classList.add('open');$('menuOv').classList.add('open')}
function closeMenu(){$('sideMenu').classList.remove('open');$('menuOv').classList.remove('open')}
function toggleMenuGroup(gid){
  _menuExpanded[gid]=!_menuExpanded[gid];
  buildMenu();
}
function _isChildActive(children){
  const cur=CUR_MAP[state.currentView]||state.currentView;
  return children.some(c=>c.id===cur||c.id===state.currentView);
}
function buildMenu(){
  const cur = CUR_MAP[state.currentView] || state.currentView;
  let items = [...menuItems];
  if(isAdminMode()){
    items.push({id:'admin-settings',icon:'lock',label:'管理者設定 (Admin)'});
  }
  const chevSvg='<svg class="menu-expand-icon" width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M9 18l6-6-6-6"/></svg>';
  let html='';
  items.forEach(m=>{
    if(m.children){
      const childActive=_isChildActive(m.children);
      const isOpen=_menuExpanded[m.id]||childActive;
      html+=`<div class="menu-group-hd${childActive?' cur':''}" onclick="toggleMenuGroup('${m.id}')">
        <span style="display:flex;align-items:center;gap:14px;flex:1">${I[m.icon]}${m.label}</span>
        <svg class="menu-expand-icon${isOpen?' open':''}" width="16" height="16" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M9 18l6-6-6-6"/></svg>
      </div>`;
      html+=`<div class="menu-children${isOpen?' open':''}">`;
      m.children.forEach(c=>{
        const isCur=c.id===cur||c.id===state.currentView;
        html+=`<a onclick="nav('${c.id}')" class="${isCur?'cur':''}">${c.ic&&I[c.ic]?I[c.ic]:''}${c.label}</a>`;
      });
      html+=`</div>`;
    }else{
      html+=`<a onclick="nav('${m.id}')" class="${m.id===cur?'cur':''}">${I[m.icon]}${m.label}</a>`;
    }
  });
  $('menuNav').innerHTML=html;
}

/* ── Admin Tab Bar ── */
function updateAdminUI(){
  const admin = isAdminMode();
  const badge = $('adminBadge');
  const tabBar = $('adminTabBar');
  if(badge) badge.style.display = admin ? 'inline-flex' : 'none';
  if(tabBar){
    const onMainViews = !['login','profile-setup'].includes(state.currentView);
    tabBar.style.display = (admin && onMainViews) ? 'flex' : 'none';
    if(state.currentView==='admin-settings'){
      $('atabMain').classList.remove('act');
      $('atabAdmin').classList.add('act');
    }else{
      $('atabMain').classList.add('act');
      $('atabAdmin').classList.remove('act');
    }
  }
}
function switchAdminTab(tab){
  if(tab==='admin'){
    renderAdminSettings();
    nav('admin-settings');
  }else{
    nav('home');
  }
}

function openSheet(title, html){
  $('sheetTitle').innerHTML=title;
  $('sheetBody').innerHTML=html;
  $('sheetOv').classList.add('open');
}
function closeSheet(){ $('sheetOv').classList.remove('open'); }
$('sheetOv') && ($('sheetOv').onclick=closeSheet);

function selGroup(cls,el){$$(`.${cls}`).forEach(e=>e.classList.remove('act'));el.classList.add('act')}

function chipGroup(field,list,multi){
  const p=state.profile||{};
  return list.map(v=>{
    const sel=multi?(Array.isArray(p[field])?p[field]:[]).includes(v):p[field]===v;
    return `<button type="button" class="tchip${sel?' act':''}" data-field="${helpers.esc(field)}" data-val="${helpers.esc(v)}" data-multi="${multi?'1':'0'}" onclick="toggleChip(this)">${helpers.esc(v)}</button>`;
  }).join('');
}
function toggleChip(el){
  if(el.dataset.multi==='1'){ el.classList.toggle('act'); }
  else{
    const f=el.dataset.field;
    document.querySelectorAll(`.tchip[data-field="${f}"]`).forEach(e=>e.classList.remove('act'));
    el.classList.add('act');
  }
}
function renderProfileFields(includeLoc){
  const p=state.profile||{}, L=state.location;
  return `
  <div class="sec-t">氏名 <small>Name</small></div>
  <div class="sbox"><div class="irow"><div class="ii">👤</div><input class="ifield" id="pfName" value="${helpers.esc(p.name||'')}" placeholder="お名前"></div></div>
  <div class="sec-t mt4">国籍 <small>Nationality</small></div>
  <div class="mb4">${chipGroup('nationality',PROFILE_OPTS.nationality,false)}</div>
  <div class="sec-t">言語 <small>複数選択可</small></div>
  <div class="mb4">${chipGroup('languages',PROFILE_OPTS.languages,true)}</div>
  <div class="sec-t">年齢 <small>Age</small></div>
  <div class="sbox"><div class="irow"><div class="ii">🎂</div><input type="number" class="ifield" id="pfAge" value="${helpers.esc(p.age||'')}" placeholder="年齢" min="0" max="120"></div></div>
  <div class="sec-t mt4">性別 <small>Gender</small></div>
  <div class="mb4">${chipGroup('gender',PROFILE_OPTS.gender,false)}</div>
  <div class="sec-t">趣向 <small>複数選択可</small></div>
  <div class="mb4">${chipGroup('preferences',PROFILE_OPTS.preferences,true)}</div>
  <div class="sec-t">日本に来た回数 <small>Visit Count</small></div>
  <div class="mb4">${chipGroup('japanVisitCount',PROFILE_OPTS.japanVisitCount,false)}</div>
  ${includeLoc?`
  <div class="sec-t mt4">位置情報 <small>Location</small></div>
  <div class="ml mb3">
    <div class="mi locPerm ${L.permission==='granted'?'act':''}" data-perm="granted" onclick="selLocPerm(this)"><div class="mi-tx">${I.loc}現在地を利用する</div><div class="radio"></div></div>
    <div class="mi locPerm ${L.permission!=='granted'?'act':''}" data-perm="denied" onclick="selLocPerm(this)"><div class="mi-tx">${I.pin}設定位置を使う</div><div class="radio"></div></div>
  </div>
  <div class="sec-t">設定位置 <small>基準位置</small></div>
  <div class="sbox"><div class="irow"><div class="ii">🏙</div><select class="ifield" id="pfFallback" style="appearance:auto">
    ${PROFILE_OPTS.cities.map(c=>`<option value="${c}" ${L.fallback===c?'selected':''}>${c}</option>`).join('')}
  </select></div></div>`:''}`;
}
function selLocPerm(el){document.querySelectorAll('.locPerm').forEach(e=>e.classList.remove('act'));el.classList.add('act')}
function collectProfile(){
  const p={...(state.profile||{})};
  p.name=($('pfName').value||'').trim();
  p.age=($('pfAge').value||'').trim();
  ['nationality','gender','japanVisitCount'].forEach(f=>{
    const el=document.querySelector(`.tchip.act[data-field="${f}"]`);
    p[f]=el?el.dataset.val:'';
  });
  ['languages','preferences'].forEach(f=>{
    p[f]=Array.from(document.querySelectorAll(`.tchip.act[data-field="${f}"]`)).map(e=>e.dataset.val);
  });
  return p;
}
async function saveProfileForm(){
  const p=collectProfile();
  if(!p.name){ helpers.toast('氏名を入力してください'); return; }
  state.profile=p;
  const lp=document.querySelector('.locPerm.act');
  const fb=$('pfFallback');
  if(fb) state.location.fallback=fb.value;
  if(lp){
    if(lp.dataset.perm==='granted'){
      helpers.toast('位置情報を取得中...');
      const c=await services.getCurrentLocation();
      if(c){ state.location.permission='granted'; state.location.coords=c; state.location.label='現在地'; }
      else{ state.location.permission='denied'; state.location.coords=null; }
    }else{
      state.location.permission='denied'; state.location.coords=null;
    }
  }
  saveState();
  helpers.toast('保存しました');
  await refreshHomeData();
  renderHome();
  nav('home');
  setTimeout(showRpgWelcome,600);
}

async function refreshHomeData(){
  const loc=services.resolveCoords();
  state.weatherForecast=await services.fetchWeather(loc.lat, loc.lon);
  state.weather=state.weatherForecast;
  state.nearbySpots=await services.fetchNearbySpots(loc.lat, loc.lon);
  renderWeatherCard(); renderNearbySpots(); renderTodoList(); renderHomeAI();
}

function renderLogin(){
  $('v-login').innerHTML=`
    <div class="login-bg">
      <div class="login-chara" style="width:90px;height:90px;margin:0 auto 20px"><img src="${getSelectedAvatar().img}" style="width:90px;height:90px;border-radius:50%;object-fit:cover;border:3px solid var(--pri);box-shadow:0 8px 24px rgba(0,0,0,.15)"></div>
      <div class="login-logo">AssisTrip<sub>AI</sub></div>
      <p class="login-welcome">Welcome to Japan！</p>
      <p style="font-size:13px;color:var(--txs);margin-bottom:12px;text-align:center">あなたの旅を一緒に歩くAIガイドが待っています</p>
      <div class="login-form">
        <div class="avatar-sel-wrap">
          <div class="avatar-sel-title">旅の案内人を選ぼう</div>
          <div class="avatar-sel-sub">あなたの旅に寄り添うパートナーを選んでください</div>
          <div class="avatar-cards" id="loginAvatarCards"></div>
        </div>
        <div class="sbox" style="margin-top:16px"><div class="irow"><div class="ii">📧</div><input class="ifield" id="loginEmail" placeholder="メールアドレス" value="${helpers.esc(state.session.email||'')}"></div></div>
        <button class="btn bp" style="padding:16px;font-size:16px;margin-top:16px;box-shadow:0 8px 24px rgba(10,132,255,.3)" onclick="doLogin()">ログイン / はじめる</button>
        <p class="txs fsub mt4 tac">※ デモ版です。実際の認証は行われません。</p>
        <div class="login-admin-toggle"><button onclick="toggleAdminLogin()">🔐 管理者としてログイン</button></div>
        <div class="login-admin-fields" id="adminLoginFields">
          <div class="sbox" style="margin-top:12px;border:2px solid #E5E5EA">
            <div class="irow"><div class="ii">${I.lock}</div><input class="ifield" id="adminIdIn" placeholder="管理者ID" autocomplete="off"></div>
            <div class="divider"></div>
            <div class="irow"><div class="ii">🔑</div><input type="password" class="ifield" id="adminPassIn" placeholder="管理者パスワード" autocomplete="off"></div>
          </div>
          <button class="btn" style="padding:14px;font-size:15px;margin-top:8px;background:linear-gradient(135deg,#FF6B6B,#EE5A24);color:#fff" onclick="doAdminLogin()">管理者ログイン</button>
        </div>
      </div>
    </div>`;
  setTimeout(renderLoginAvatars,0);
}
function renderLoginAvatars(){
  const cur=getAdminSetting('avatar','tsumugi');
  const el=$('loginAvatarCards');
  if(!el) return;
  el.innerHTML=AVATARS.map(a=>`<div class="av-card${a.id===cur?' sel':''}" onclick="selectLoginAvatar('${a.id}')">
    <div class="av-check">✓</div>
    <img class="av-img" src="${a.img}" alt="${helpers.esc(a.name)}">
    <div class="av-nm">${helpers.esc(a.name)}</div>
    <div class="av-desc">${helpers.esc(a.shortDesc)}</div>
  </div>`).join('');
}
function selectLoginAvatar(id){
  setAdminSetting('avatar',id);
  renderLoginAvatars();
  /* Preview theme */
  applyAvatarTheme();
}
function toggleAdminLogin(){
  const el=$('adminLoginFields');
  if(el) el.classList.toggle('open');
}
function doLogin(){
  const em=($('loginEmail').value||'').trim();
  state.session.isLoggedIn=true;
  state.session.email=em||'guest@assistrip';
  setAdminMode(false);
  saveState();
  applyAvatarTheme();
  updateAvatarUI();
  if(!state.profile||!state.profile.name){ renderProfileSetup(); nav('profile-setup'); }
  else{ renderHome(); renderSettings(); nav('home'); refreshHomeData(); setTimeout(showRpgWelcome,600); }
}
function doAdminLogin(){
  const id=($('adminIdIn').value||'').trim();
  const pw=($('adminPassIn').value||'').trim();
  if(id==='nttkk' && pw==='nttkk@000'){
    const em=($('loginEmail').value||'').trim();
    state.session.isLoggedIn=true;
    state.session.email=em||'admin@assistrip';
    setAdminMode(true);
    saveState();
    helpers.toast('管理者としてログインしました');
    applyAvatarTheme(); updateAvatarUI();
    if(!state.profile||!state.profile.name){ renderProfileSetup(); nav('profile-setup'); }
    else{ renderHome(); renderSettings(); nav('home'); refreshHomeData(); setTimeout(showRpgWelcome,600); }
  }else{
    helpers.toast('管理者IDまたはパスワードが違います');
  }
}
function renderProfileSetup(){
  $('v-profile-setup').innerHTML=`<div class="sh"><div style="width:32px"></div><h2>プロフィール登録</h2></div>
    <section class="sec">
      <div class="chara-msg"><img class="chara-av" src="${getSelectedAvatar().img}" alt=""><div class="bub">旅のご案内のため、少し教えてください。登録内容はいつでも設定から変更できます。</div></div>
      ${renderProfileFields(true)}
      <button class="btn bp mt4" style="padding:16px;font-size:16px;margin-top:24px" onclick="saveProfileForm()">登録してはじめる</button>
    </section>`;
}
function renderSettings(){
  const curAv=getSelectedAvatar();
  $('v-settings').innerHTML=helpers.sh('home','設定')+`
    <section class="sec">
      <div class="sec-t">AIガイド <small>Avatar</small></div>
      <div class="settings-av-row">${AVATARS.map(a=>`<div class="settings-av-opt${a.id===curAv.id?' act':''}" onclick="setSelectedAvatar('${a.id}');renderSettings();renderHome();initChatGreeting()">
        <img src="${a.img}" alt="${helpers.esc(a.name)}"><div class="nm">${helpers.esc(a.name)}</div>
      </div>`).join('')}</div>
      ${renderProfileFields(true)}
      <button class="btn bp mt4" style="padding:16px;font-size:16px;margin-top:24px" onclick="saveProfileForm()">変更を保存</button>
      <button class="btn bo mt3" style="border-color:var(--red);color:var(--red);padding:14px;margin-top:12px" onclick="doLogout()">ログアウト</button>
    </section>`;
}
function doLogout(){
  state.session.isLoggedIn=false; chatHistory.length=0;
  setAdminMode(false);
  saveState(); renderLogin(); nav('login');
}

/* ── Admin Settings View ── */
function renderAdminSettings(){
  const provider = getAdminSetting('aiProvider','claude');
  const openaiKey = getAdminSetting('openAiApiKey','');
  const geminiKey = getAdminSetting('geminiApiKey','');
  const claudeKey = getAdminSetting('claudeApiKey','');
  const mapsKey   = getAdminSetting('googleMapsApiKey','');
  const sysPrompt = getAdminSetting('aiSystemPrompt','');
  const lastSaved = getAdminSetting('lastSaved','');

  $('v-admin-settings').innerHTML=helpers.sh('home','管理者設定')+`<section class="sec">

    <div class="chara-msg"><img class="chara-av" src="${getSelectedAvatar().img}" alt=""><div class="bub">管理者設定です。ここで設定したAPIキーやプロバイダはlocalStorageに保存され、メイン画面で自動的に使用されます。</div></div>

    ${lastSaved?`<p class="txs fsub mb3">最終保存: ${helpers.esc(lastSaved)}</p>`:''}

    <!-- 1. AI Provider -->
    <div class="admin-section">
      <h3>🤖 AIプロバイダ選択</h3>
      <p class="adesc">メイン画面のAIコンシェルジュで使用するAIプロバイダを選択してください。</p>
      <div class="admin-field">
        <label>プロバイダ</label>
        <div class="af-input-wrap">
          <select id="admProvider">
            <option value="openai" ${provider==='openai'?'selected':''}>OpenAI</option>
            <option value="gemini" ${provider==='gemini'?'selected':''}>Gemini</option>
            <option value="claude" ${provider==='claude'?'selected':''}>Claude</option>
          </select>
        </div>
      </div>
    </div>

    <!-- 2. API Keys -->
    <div class="admin-section">
      <h3>🔑 APIキー設定</h3>
      <p class="adesc">各プロバイダのAPIキーを入力してください。入力欄はセキュリティのためパスワード表示です。</p>

      <div class="admin-field">
        <label>OpenAI APIキー</label>
        <div class="af-input-wrap">
          <input type="password" id="admOpenAiKey" value="${helpers.esc(openaiKey)}" placeholder="sk-...">
          <button class="toggle-vis" onclick="toggleKeyVis('admOpenAiKey',this)" title="表示/非表示">👁</button>
        </div>
      </div>

      <div class="admin-field">
        <label>Gemini APIキー</label>
        <div class="af-input-wrap">
          <input type="password" id="admGeminiKey" value="${helpers.esc(geminiKey)}" placeholder="AIza...">
          <button class="toggle-vis" onclick="toggleKeyVis('admGeminiKey',this)" title="表示/非表示">👁</button>
        </div>
      </div>

      <div class="admin-field">
        <label>Claude APIキー</label>
        <div class="af-input-wrap">
          <input type="password" id="admClaudeKey" value="${helpers.esc(claudeKey)}" placeholder="sk-ant-...">
          <button class="toggle-vis" onclick="toggleKeyVis('admClaudeKey',this)" title="表示/非表示">👁</button>
        </div>
      </div>

      <div class="admin-field">
        <label>Google Maps APIキー</label>
        <div class="af-input-wrap">
          <input type="password" id="admMapsKey" value="${helpers.esc(mapsKey)}" placeholder="AIza...">
          <button class="toggle-vis" onclick="toggleKeyVis('admMapsKey',this)" title="表示/非表示">👁</button>
        </div>
      </div>
    </div>

    <!-- 3. System Prompt -->
    <div class="admin-section">
      <h3>📝 AIシステムプロンプト</h3>
      <p class="adesc">AIの役割・口調・返答ルールを定義します。空の場合はデフォルトが使用されます。</p>
      <div class="admin-field">
        <label>システムプロンプト</label>
        <div class="af-input-wrap">
          <textarea id="admSysPrompt" placeholder="例: あなたは親切な旅行コンシェルジュです...">${helpers.esc(sysPrompt)}</textarea>
        </div>
      </div>
    </div>

    <!-- 4. API Key Help -->
    <div class="admin-section">
      <h3>📖 APIキーの取得方法</h3>

      <div class="api-help-card">
        <div class="ahc-title">🟢 OpenAI APIキー</div>
        <a href="https://platform.openai.com/settings/organization/api-keys" target="_blank" rel="noopener noreferrer">${I.ext} platform.openai.com で取得</a>
      </div>

      <div class="api-help-card">
        <div class="ahc-title">🔵 Gemini APIキー</div>
        <a href="https://aistudio.google.com/apikey" target="_blank" rel="noopener noreferrer">${I.ext} aistudio.google.com で取得</a>
        <div class="ahc-note"><a href="https://ai.google.dev/gemini-api/docs/api-key" target="_blank" rel="noopener noreferrer">補足ドキュメント</a></div>
      </div>

      <div class="api-help-card">
        <div class="ahc-title">🟠 Claude APIキー</div>
        <a href="https://console.anthropic.com/" target="_blank" rel="noopener noreferrer">${I.ext} console.anthropic.com で取得</a>
        <div class="ahc-note"><a href="https://docs.anthropic.com/en/docs/get-started" target="_blank" rel="noopener noreferrer">補足ドキュメント</a></div>
      </div>

      <div class="api-help-card">
        <div class="ahc-title">🗺️ Google Maps APIキー</div>
        <a href="https://developers.google.com/maps/documentation/embed/get-api-key" target="_blank" rel="noopener noreferrer">${I.ext} Embed API キー取得</a>
        <div class="ahc-note"><a href="https://developers.google.com/maps/documentation/javascript/get-api-key" target="_blank" rel="noopener noreferrer">JavaScript API キー取得</a></div>
      </div>
    </div>

    <!-- Save Button -->
    <button class="btn bp" style="padding:16px;font-size:16px" onclick="saveAdminSettings()">設定を保存</button>

  </section>`;
}
function toggleKeyVis(inputId, btn){
  const inp=$(inputId);
  if(!inp) return;
  if(inp.type==='password'){ inp.type='text'; btn.textContent='🙈'; }
  else{ inp.type='password'; btn.textContent='👁'; }
}
function saveAdminSettings(){
  const provider = $('admProvider').value;
  const openaiKey = $('admOpenAiKey').value.trim();
  const geminiKey = $('admGeminiKey').value.trim();
  const claudeKey = $('admClaudeKey').value.trim();
  const mapsKey   = $('admMapsKey').value.trim();
  const sysPrompt = $('admSysPrompt').value;

  setAdminSetting('aiProvider', provider);
  setAdminSetting('openAiApiKey', openaiKey);
  setAdminSetting('geminiApiKey', geminiKey);
  setAdminSetting('claudeApiKey', claudeKey);
  setAdminSetting('googleMapsApiKey', mapsKey);
  setAdminSetting('aiSystemPrompt', sysPrompt);
  setAdminSetting('lastSaved', new Date().toLocaleString('ja-JP'));

  helpers.toast('管理者設定を保存しました');
}

function renderHome(){
  const p=state.profile||{};
  const name=p.name||'ゲスト';
  const daysLabel=p.japanVisitCount?`🇯🇵 ${p.japanVisitCount}の訪問`:'🇯🇵 日本滞在中';
  const av=getSelectedAvatar();
  $('homeGreeting').innerHTML=`<div style="padding:16px 20px 8px">
    <h1 style="font-size:24px;font-weight:800;letter-spacing:-.5px;margin-bottom:4px">こんにちは、${helpers.esc(name)}さん</h1>
    <div style="display:inline-block;background:#E5E5EA;padding:4px 12px;border-radius:20px;font-size:12px;font-weight:600">${daysLabel}</div>
  </div>`;
  renderWeatherCard(); renderNearbySpots(); renderTodoList(); renderHomeAI();
  const qItems=[
    {v:'mobility-hub',icon:'route',l:'経路・チケット',sub:'Mobility Gate'},
    {v:'baggage',icon:'bag',l:'手荷物配送',sub:'Baggage Delivery'},
    {v:'tour',icon:'tour',l:'観光ガイド',sub:'Smart Tour'},
    {v:'trouble',icon:'sos',l:'トラブル・SOS',sub:'Help & Support',danger:true}
  ];
  $('quickGrid').innerHTML=qItems.map(q=>`<button class="qbtn" onclick="nav('${q.v}')"><div class="icn-c" ${q.danger?'style="background:var(--red-bg);color:var(--red)"':''}>${I[q.icon]}</div><span>${q.l}<br><small class="fsub">${q.sub}</small></span></button>`).join('');
  const links=[
    {v:'refund',icon:'yen',l:'免税リファンド (Tax-Free Refund)'},
    {v:'oac',icon:'plane',l:'空港チェックイン (OAC)'},
    {v:'settings',icon:'gear',l:'設定 (Settings)'}
  ];
  $('homeLinks').innerHTML=links.map(l=>`<div class="mi" onclick="nav('${l.v}')"><div class="mi-tx">${I[l.icon]}${l.l}</div>${I.chev}</div>`).join('');
}
function renderWeatherCard(){
  const el=$('homeWeather'); if(!el) return;
  const loc=services.resolveCoords();
  const w=state.weather?.current;
  if(!w){
    el.innerHTML=`<div class="wcard" onclick="refreshHomeData()"><div class="wi">🌐</div><div class="wbody"><div class="wloc">${helpers.esc(loc.label)}</div><div class="wt" style="font-size:14px">タップして天気を取得</div></div></div>`;
    return;
  }
  const m=helpers.mapWeatherToIcon(w.code);
  const range=(w.tempMin!=null&&w.tempMax!=null)?`↑${w.tempMax}° / ↓${w.tempMin}°`:'';
  el.innerHTML=`<div class="wcard ${m.cls}" onclick="openWeatherModal()">
    <div class="wi">${m.em}</div>
    <div class="wbody">
      <div class="wloc">${helpers.esc(loc.label)} ・ ${helpers.esc(m.label)}</div>
      <div class="wt">${w.temp}<small>℃</small></div>
      <div class="wrange">${range}</div>
      <div class="wo">👕 ${helpers.esc(helpers.getClothingAdvice(w.temp,w.code))}</div>
    </div>
  </div>`;
}
function renderNearbySpots(){
  const el=$('homeNearby'); if(!el) return;
  const list=state.nearbySpots.slice(0,5);
  if(!list.length){
    el.innerHTML=`<div class="nsc" onclick="refreshHomeData()">
      <div class="nsc-hd"><span class="t">${I.pin} 近くのおすすめスポット</span></div>
      <p class="nsc-empty">スポットを取得中です。タップして再取得できます。</p>
    </div>`;
    return;
  }
  el.innerHTML=`<div class="nsc">
    <div class="nsc-hd"><span class="t">${I.pin} 近くのおすすめスポット</span><span class="more">${list.length}件</span></div>
    <div class="nsc-scroll">
      ${list.map((s,idx)=>`<div class="nsc-item" onclick="openSpotModal(state.nearbySpots[${idx}])">
        <span class="ct">${s.emoji||''} ${helpers.esc(s.category)}</span>
        <div class="nm">${helpers.esc(s.name)}</div>
        <div class="ds">${helpers.formatDistance(s.distanceKm)} ・ ${helpers.esc((s.desc||'').slice(0,22))}</div>
      </div>`).join('')}
    </div>
  </div>`;
}
function renderTodoList(){
  const el=$('todoList'); if(!el) return;
  const list=visibleTodos();
  if(!list.length){
    el.innerHTML=`<div class="empty-todo">✓ 現在、未完了のToDoはありません</div>`;
    return;
  }
  el.innerHTML=list.map(t=>`<div class="todo-card" onclick="openTodoDetail('${t.id}')">
    <div class="sa-i">${t.icon}</div>
    <div class="sa-body"><div class="t">${helpers.esc(t.title)}</div><div class="s">${helpers.esc(t.desc)}</div></div>
    <div class="sa-arrow">${I.chev}</div>
  </div>`).join('');
}

function openTodoDetail(id){
  const def = TODO_DEFS.find(t=>t.id===id); if(!def) return;
  state.selectedTodo = id;
  const key='todoChecks_'+id;
  let checks=[]; try{ checks=JSON.parse(localStorage.getItem(key)||'[]'); }catch(e){}
  const isChecked = i => checks.includes(i);
  const html = helpers.sh('home', def.title) + `<section class="sec">
    <div class="chara-msg"><img class="chara-av" src="${getSelectedAvatar().img}" alt=""><div class="bub">${helpers.esc(def.desc)} 完了したら「すべて完了」を押してください。</div></div>
    <div class="card">
      ${def.items.map((txt,i)=>`<label class="fx aic g3 mb3" style="cursor:pointer">
        <input type="checkbox" class="ckb todo-ck" data-i="${i}" ${isChecked(i)?'checked':''}>
        <span class="ts fw7">${helpers.esc(txt)}</span>
      </label>`).join('')}
    </div>
    ${def.link?`<button class="btn bo mb3" onclick="nav('${def.link.view}')">${helpers.esc(def.link.label)}</button>`:''}
    <button class="btn bp" onclick="completeTodo('${id}')">すべて完了にする</button>
  </section>`;
  $('v-todo-detail').innerHTML = html;
  nav('todo-detail');
  setTimeout(()=>{
    $$('.todo-ck').forEach(c=>c.addEventListener('change',()=>{
      const checked=Array.from($$('.todo-ck')).filter(x=>x.checked).map(x=>parseInt(x.dataset.i));
      try{ localStorage.setItem(key, JSON.stringify(checked)); }catch(e){}
    }));
  },0);
}
function completeTodo(id){
  state.completedTodos[id]=true;
  saveState();
  helpers.toast('ToDoを完了しました');
  renderTodoList();
  nav('home');
}

function openSpotModal(sp){
  if(!sp) return;
  state.selectedSpot=sp;
  const q=encodeURIComponent(sp.name);
  const mapUrl = sp.lat && sp.lon
    ? `https://www.google.com/maps/search/?api=1&query=${sp.lat},${sp.lon}(${q})`
    : `https://www.google.com/maps/search/?api=1&query=${q}`;
  const searchUrl=`https://www.google.com/search?q=${q}`;
  const websiteHtml=sp.website?`<a class="sm-link" href="${helpers.esc(sp.website)}" target="_blank" rel="noopener noreferrer"><span class="ic">${I.ext}</span>公式サイトを開く<span class="ar">${I.chev}</span></a>`:'';
  const openingHtml=sp.opening?`<div class="wd-row"><span>営業時間</span><span>${helpers.esc(sp.opening)}</span></div>`:'';
  const html=`
    <div class="sm-cat">${sp.emoji||'📍'} ${helpers.esc(sp.category)}</div>
    <div class="sm-h">${helpers.esc(sp.name)}</div>
    <div class="sm-sub">${helpers.formatDistance(sp.distanceKm)} から</div>
    <div class="sm-desc">${helpers.esc(sp.desc||'詳細な情報は下記リンクからご確認いただけます。')}</div>
    ${openingHtml?`<div class="card flat" style="padding:8px 12px;margin-bottom:16px">${openingHtml}</div>`:''}
    <div class="sm-links">
      <a class="sm-link" href="${helpers.esc(mapUrl)}" target="_blank" rel="noopener noreferrer"><span class="ic">${I.pin}</span>Google Mapsで開く<span class="ar">${I.chev}</span></a>
      ${websiteHtml}
      <a class="sm-link" href="${helpers.esc(searchUrl)}" target="_blank" rel="noopener noreferrer"><span class="ic">${I.search}</span>Webで検索<span class="ar">${I.chev}</span></a>
    </div>
    <button class="btn bp mb3" onclick="routeFromSpot()">${I.route} このスポットへの経路を開く</button>
    <button class="btn bo" onclick="closeSheet();nav('tour')">${I.tour} 観光提案を見る</button>
  `;
  openSheet(`${I.pin} スポット詳細`, html);
}
function routeFromSpot(){
  const sp=state.selectedSpot; if(!sp) return;
  state.mobility.destination=sp.name;
  saveState();
  closeSheet();
  renderMobility(); nav('mobility');
}

function openWeatherModal(){
  state.weatherDetailTab='today';
  renderWeatherModal();
  $('sheetOv').classList.add('open');
}
function renderWeatherModal(){
  const f=state.weatherForecast;
  if(!f){ openSheet('天気', `<p class="fsub ts">天気情報を取得中です。</p>`); return; }
  const tab=state.weatherDetailTab;
  const loc=services.resolveCoords();
  const w=f.current;
  const m=helpers.mapWeatherToIcon(w.code);
  let body=`<div class="wd-tabs">${['today','hourly','weekly'].map(k=>`<button class="wd-tab${k===tab?' act':''}" onclick="state.weatherDetailTab='${k}';renderWeatherModal()">${{today:'今日',hourly:'1時間ごと',weekly:'週間'}[k]}</button>`).join('')}</div>`;
  if(tab==='today'){
    body+=`<div class="wd-hero"><div class="ic">${m.em}</div><div class="tp">${w.temp}°</div><div class="cd">${helpers.esc(m.label)} ・ ${helpers.esc(loc.label)}</div></div>
    <div class="card flat">
      <div class="wd-row"><span>最高 / 最低</span><span>${w.tempMax??'-'}° / ${w.tempMin??'-'}°</span></div>
      <div class="wd-row"><span>湿度</span><span>${w.humidity??'-'}%</span></div>
      <div class="wd-row"><span>風速</span><span>${w.wind??'-'} m/s</span></div>
      <div class="wd-row"><span>服装</span><span>${helpers.esc(helpers.getClothingAdvice(w.temp,w.code))}</span></div>
    </div>`;
  }else if(tab==='hourly'){
    body+=`<div class="wd-hour">${f.hourly.map(h=>{
      const hi=helpers.mapWeatherToIcon(h.code);
      return `<div class="wd-hitem"><div class="h">${h.time.getHours()}時</div><div class="i">${hi.em}</div><div class="t">${h.temp}°</div></div>`;
    }).join('')}</div><p class="txs fsub mt4">※ 今後12時間の予報</p>`;
  }else{
    body+=`<div class="card flat">${f.daily.map((d,i)=>{
      const hi=helpers.mapWeatherToIcon(d.code);
      const lbl=i===0?'今日':helpers.dayLabel(d.date)+' '+helpers.fmtDate(d.date);
      return `<div class="wd-day"><div class="d">${lbl}</div><div class="i">${hi.em}</div><div class="c">${helpers.esc(hi.label)}</div><div class="r">${d.max}° / ${d.min}°</div></div>`;
    }).join('')}</div>`;
  }
  openSheet(`${m.em} 天気詳細`, body);
}

function updBal(){$$('.js-bal').forEach(e=>{e.textContent='¥ '+state.balance.toLocaleString()})}
function renderPayTop(){
  $('v-pay-top').innerHTML=helpers.sh('home','交通・決済')+`<section class="sec">
  <div class="pay-card" style="cursor:default"><div class="fx jcsb aic mb4"><span class="fw7">連携中のカード</span><span class="pay-status">利用可能</span></div><div class="pay-label">IC残高</div><div class="pay-bal js-bal">¥ ${state.balance.toLocaleString()}</div></div>
  <div class="ml">${[{v:'charge',i:'plus',l:'チャージする'},{v:'tap',i:'yen',l:'かざして使う'},{v:'ic-manage',i:'lock',l:'ICカード連携・管理'}].map(m=>`<div class="mi" onclick="nav('${m.v}')"><div class="mi-tx">${I[m.i]}${m.l}</div>${I.chev}</div>`).join('')}</div>
  <div class="sec-t mt4">乗り方案内 <small>How to ride</small></div>
  <div class="card"><div class="gi"><div class="gi-icon">${I.flag}</div><div><h4>在来線・地下鉄・バス</h4><p>チャージ残高があれば「かざして使う」で改札を通れます。</p></div></div><div class="gi"><div class="gi-icon" style="background:var(--red-bg);color:var(--red)">${I.bolt}</div><div><h4>新幹線・一部の特急</h4><p>ICカードだけでは乗れません。経路・チケットから予約が必要です。</p></div></div>
  <button class="btn mt3" style="color:var(--pri);background:#F0F8FF" onclick="nav('mobility-hub')">経路・チケットを開く</button></div></section>`;
}
function renderCharge(){
  $('v-charge').innerHTML=helpers.sh('pay-top','チャージ')+`<section class="sec">
  <div class="fxc aic mb4"><span class="fsub ts">現在の残高</span><span class="fw7 js-bal" style="font-size:32px">¥ ${state.balance.toLocaleString()}</span></div>
  <div class="sec-t mt4">金額を選択</div>
  <div class="sel-grid">${[1000,3000,5000,10000].map(a=>`<div class="sel-btn chrg${a===state.chargeAmt?' act':''}" onclick="pickCharge(${a},this)">¥ ${a.toLocaleString()}</div>`).join('')}</div>
  <div class="sec-t">支払い方法</div>
  <div class="ml"><div class="mi pm act" onclick="selGroup('pm',this)"><div class="mi-tx">${I.card}Apple Pay</div><div class="radio"></div></div><div class="mi pm" onclick="selGroup('pm',this)"><div class="mi-tx">${I.card}Visa **** 1234</div><div class="radio"></div></div></div>
  <button class="btn bp mt4" style="padding:16px;font-size:16px" onclick="doCharge()" id="chrgBtn">¥ ${state.chargeAmt.toLocaleString()} をチャージ</button></section>`;
}
function pickCharge(a,el){state.chargeAmt=a;selGroup('chrg',el);$('chrgBtn').textContent=`¥ ${a.toLocaleString()} をチャージ`}
function doCharge(){state.balance+=state.chargeAmt;updBal();helpers.toast(`¥ ${state.chargeAmt.toLocaleString()} をチャージしました`);renderPayTop();renderTodoList();nav('pay-top')}
function renderTap(){
  $('v-tap').innerHTML=`<div class="sh"><button class="back" onclick="nav('pay-top')">${I.back}</button></div><section class="sec tap-area"><div style="font-size:20px;font-weight:800;color:var(--grn);margin-bottom:8px">利用準備完了</div><div class="fsub" style="font-size:14px;margin-bottom:40px">改札のリーダーにスマホをかざしてください</div><div class="ic-gfx"><div class="ic-lg">Travel IC</div><div class="ic-mk"></div></div><div class="pay-label" style="color:var(--txs)">現在の残高</div><div class="js-bal" style="font-size:40px;font-weight:800;margin-bottom:40px">¥ ${state.balance.toLocaleString()}</div><button class="btn bp" style="width:80%" onclick="helpers.toast('NFCリーダー起動 (Mock)')">NFCリーダーを手動起動</button></section>`;
}
function renderIcManage(){
  $('v-ic-manage').innerHTML=helpers.sh('pay-top','ICカード連携・管理')+`<section class="sec"><div class="sec-t">現在の連携状態</div><div class="card fx jcsb aic"><div class="fx aic g2"><div class="gi-icon">${I.card}</div><span class="fw7">Travel IC (Suica)</span></div><span class="badge b-grn">連携済み</span></div>
  <div class="sec-t mt4">新しく連携する <small>Add Card</small></div><div class="ml">${[{l:'モバイルPASMO',s:'すでにお持ちのPASMOを登録'},{l:'モバイルICOCA',s:'西日本エリアで便利なICOCA'}].map(c=>`<div class="mi" onclick="helpers.toast('${c.l}の連携フローを開始します')"><div class="fxc"><div class="mi-tx">${c.l}を追加</div><div class="mi-sub">${c.s}</div></div>${I.chev}</div>`).join('')}</div></section>`;
}

function renderMobilityHub(){
  $('v-mobility-hub').innerHTML=helpers.sh('home','経路・チケット')+`<section class="sec">
    <div class="chara-msg"><img class="chara-av" src="${getSelectedAvatar().img}" alt=""><div class="bub">どちらをご用意しましょう？ルート検索か、乗車券・チケットの購入を選んでください。</div></div>
    <div class="hub-opt" onclick="nav('mobility');renderMobility()">
      <div class="ic">${I.route}</div>
      <div class="body"><div class="t">ルート検索</div><div class="s">出発地・目的地・移動手段から経路を調べる</div></div>
      ${I.chev}
    </div>
    <div class="hub-opt" onclick="openTicketFromMode(null)">
      <div class="ic">${I.ticket}</div>
      <div class="body"><div class="t">乗車券・チケットの購入</div><div class="s">新幹線・高速バス・1日乗車券など</div></div>
      ${I.chev}
    </div>
  </section>`;
}

function renderMobility(){
  const M=state.mobility;
  const canUseCurrent = state.location.permission==='granted' && state.location.coords;
  const defOrigin = M.origin || (canUseCurrent?'現在地':'');
  const catBtns = MODE_GROUPS.map(g=>`<button type="button" class="${M.category===g.k?'act':''}" onclick="setMobilityCat('${g.k}')">${helpers.esc(g.l)}</button>`).join('');
  const currentGroup = MODE_GROUPS.find(g=>g.k===M.category) || MODE_GROUPS[0];
  const subBtns = currentGroup.subs.map(s=>`<button type="button" class="${M.mode===s.k?'act':''}" onclick="setMobilityMode('${s.k}')"><span class="em">${s.em}</span><span>${helpers.esc(s.l)}</span></button>`).join('');

  $('v-mobility').innerHTML=helpers.sh('mobility-hub','ルート検索 (Route)')+`<section class="sec">
    <div class="sbox">
      <div class="irow"><div class="ii">${I.loc}</div><input class="ifield" id="origIn" placeholder="出発地 (Origin) ※空欄可" value="${helpers.esc(defOrigin)}"></div>
      <div class="divider"></div>
      <div class="irow"><div class="ii">${I.pin}</div><input class="ifield" id="destIn" placeholder="目的地 (Destination)" value="${helpers.esc(M.destination||'')}"></div>
    </div>
    <button class="btn bo mb4" style="padding:10px;font-size:13px" onclick="useCurrentAsOrigin()">${I.loc} 現在地を出発地に</button>

    <div class="sec-t">移動手段 <small>Travel Mode</small></div>
    <div class="mode-cat">${catBtns}</div>
    <div class="mode-sub">${subBtns}</div>

    <div class="sec-t">経路プレビュー <small>Route Preview</small></div>
    <div class="map-wrap" id="mapWrap">${renderMapEmbed()}</div>

    <button class="btn bp mb3" onclick="searchRoute()">${I.search} この条件で検索</button>
    <button class="btn bo mb3" onclick="openRouteExt()">${I.ext} Google Mapsで大きく開く</button>
    <button class="btn bp mb4" style="background:var(--org)" onclick="openTicketFromMode('${M.mode}')">${I.ticket} 乗車券・チケットの購入に進む</button>

    <div class="sec-t mt4">よく使う目的地 <small>Favorites</small></div>
    <div class="ml">${['新宿駅','浅草寺','渋谷駅','東京駅','箱根温泉'].map(d=>`<div class="mi" onclick="pickFav('${d}')"><div class="mi-tx">${I.pin}${d}</div>${I.chev}</div>`).join('')}</div>
  </section>`;
}
function renderMapEmbed(){
  const M=state.mobility;
  let origin='';
  if(M.origin==='現在地' && state.location.coords) origin=`${state.location.coords.lat},${state.location.coords.lon}`;
  else if(M.origin) origin=M.origin;
  const dest=M.destination||'';
  if(!dest){
    return `<div class="map-fallback"><div style="font-size:36px">🗺️</div><div class="ts fsub">目的地を入力して検索してください。</div></div>`;
  }
  const embedUrl = buildMapsEmbedURL(origin, dest, M.mode);
  if(!embedUrl){
    return `<div class="map-fallback"><div style="font-size:36px">🗺️</div><div class="ts fsub" style="max-width:260px">Google Maps埋め込みAPIキーが未設定です。<br>管理者設定からAPIキーを設定するか、下のボタンから外部マップを開けます。</div></div>`;
  }
  return `<iframe loading="lazy" allowfullscreen referrerpolicy="no-referrer-when-downgrade" src="${helpers.esc(embedUrl)}"></iframe>`;
}
function setMobilityCat(k){
  state.mobility.category=k;
  const g=MODE_GROUPS.find(x=>x.k===k);
  if(g && !g.subs.find(s=>s.k===state.mobility.mode)) state.mobility.mode=g.subs[0].k;
  renderMobility();
}
function setMobilityMode(k){ state.mobility.mode=k; renderMobility(); updateMapEmbed(); }
function updateMapEmbed(){ const wrap=$('mapWrap'); if(wrap) wrap.innerHTML=renderMapEmbed(); }
function pickFav(d){
  const di=$('destIn'); if(di) di.value=d;
  state.mobility.destination=d;
  updateMapEmbed();
}
function useCurrentAsOrigin(){
  if(state.location.permission!=='granted'||!state.location.coords){ helpers.toast('位置情報が未設定です。設定から有効化してください'); return; }
  const oi=$('origIn'); if(oi) oi.value='現在地';
  state.mobility.origin='現在地';
}
function searchRoute(){
  const orig=($('origIn').value||'').trim();
  const dest=($('destIn').value||'').trim();
  if(!dest){ helpers.toast('目的地を入力してください'); return; }
  state.mobility.origin=orig; state.mobility.destination=dest; saveState();
  updateMapEmbed();
}
function openRouteExt(){
  const orig=($('origIn')?.value||state.mobility.origin||'').trim();
  const dest=($('destIn')?.value||state.mobility.destination||'').trim();
  if(!dest){ helpers.toast('目的地を入力してください'); return; }
  let originParam='';
  if(orig==='現在地' && state.location.coords) originParam=`${state.location.coords.lat},${state.location.coords.lon}`;
  else if(orig) originParam=orig;
  const url=buildMapsExternalURL(originParam, dest, state.mobility.mode);
  openExt(url);
}

const TICKETS = [
  {id:'shinkansen', name:'新幹線チケット', em:'🚅', price:13320, desc:'主要区間の新幹線指定席券(目安料金)', tagModes:['shinkansen','train']},
  {id:'hwybus',     name:'高速バスチケット', em:'🚌', price:4200,  desc:'主要都市間の高速バス(片道)', tagModes:['bus']},
  {id:'bus1day',    name:'バス1日乗車券', em:'🎟️', price:600,   desc:'都バス等の1日乗り放題', tagModes:['bus']},
  {id:'airport',    name:'空港アクセス特急券', em:'✈️', price:2800,  desc:'成田/羽田/関空などへの特急', tagModes:['flight']},
  {id:'citypass',   name:'都市周遊パス', em:'🗺️', price:1800,  desc:'主要観光路線が1日乗り放題', tagModes:['train','bus']}
];
function openTicketFromMode(modeKey){
  state.ticket.highlight = modeKey || null;
  const rec = modeKey ? TICKETS.find(t=>t.tagModes.includes(modeKey)) : null;
  state.ticket.selectedId = rec ? rec.id : TICKETS[0].id;
  renderTicket();
  nav('ticket');
}
function renderTicket(){
  const t=state.ticket;
  const sel=TICKETS.find(x=>x.id===t.selectedId)||TICKETS[0];
  const total = sel.price * t.adult + Math.floor(sel.price*0.5) * t.child;
  const highlightMode=t.highlight;
  $('v-ticket').innerHTML=helpers.sh('mobility-hub','乗車券・チケット購入')+`<section class="sec">
    <div class="chara-msg"><img class="chara-av" src="${getSelectedAvatar().img}" alt=""><div class="bub">${highlightMode?`「${helpers.esc(findModeMeta(highlightMode).l)}」に合うチケットをおすすめしています。`:'ご利用になるチケットをお選びください。'}</div></div>
    <div class="sec-t">チケット種別 <small>Select Ticket</small></div>
    ${TICKETS.map(tk=>{
      const rec = highlightMode && tk.tagModes.includes(highlightMode);
      const act = tk.id===t.selectedId;
      return `<div class="ticket-card ${act?'act':''} ${rec && !act?'rec':''}" onclick="pickTicket('${tk.id}')">
        <div class="em">${tk.em}</div>
        <div class="body">
          <div class="t">${helpers.esc(tk.name)} ${rec?'<span class="badge b-org" style="font-size:10px">おすすめ</span>':''}</div>
          <div class="s">${helpers.esc(tk.desc)}</div>
          <div class="p">¥ ${tk.price.toLocaleString()} / 大人1名</div>
        </div>
      </div>`;
    }).join('')}
    <div class="sec-t mt4">ご利用詳細 <small>Details</small></div>
    <div class="sbox">
      <div class="irow"><div class="ii">${I.cal}</div><input type="date" class="ifield" id="tkDate" value="${helpers.esc(t.date)}"></div>
    </div>
    <div class="card">
      <div class="qty-row"><span class="l">大人 (Adult)</span>
        <div class="qty-ctrl"><button onclick="changeQty('adult',-1)">−</button><span class="n" id="qAdult">${t.adult}</span><button onclick="changeQty('adult',1)">+</button></div>
      </div>
      <div class="qty-row"><span class="l">子ども (Child)</span>
        <div class="qty-ctrl"><button onclick="changeQty('child',-1)">−</button><span class="n" id="qChild">${t.child}</span><button onclick="changeQty('child',1)">+</button></div>
      </div>
    </div>
    <div class="card">
      <div class="fx jcsb aic mb2"><span class="ts fsub">選択中</span><span class="fw7 ts">${helpers.esc(sel.name)}</span></div>
      <div class="fx jcsb aic"><span class="ts fsub">合計金額</span><span class="fw7" style="font-size:22px;color:var(--pri-dk)" id="ticketTotal">¥ ${total.toLocaleString()}</span></div>
    </div>
    <button class="btn bp" style="padding:16px;font-size:16px" onclick="goTicketConfirm()">購入を確認する</button>
  </section>`;
  setTimeout(()=>{
    const di=$('tkDate'); if(di) di.addEventListener('change',e=>{ state.ticket.date=e.target.value; });
  },0);
}
function pickTicket(id){ state.ticket.selectedId=id; renderTicket(); }
function changeQty(kind,delta){
  if(kind==='adult') state.ticket.adult = Math.max(1, Math.min(9, state.ticket.adult+delta));
  else state.ticket.child = Math.max(0, Math.min(9, state.ticket.child+delta));
  renderTicket();
}
function goTicketConfirm(){
  const t=state.ticket;
  const sel=TICKETS.find(x=>x.id===t.selectedId);
  const total = sel.price * t.adult + Math.floor(sel.price*0.5) * t.child;
  $('v-ticket-confirm').innerHTML=helpers.sh('ticket','購入確認')+`<section class="sec">
    <div class="card">
      <div class="fx aic g3 mb3"><div class="em" style="font-size:32px">${sel.em}</div><div><div class="fw7">${helpers.esc(sel.name)}</div><div class="ts fsub">${helpers.esc(sel.desc)}</div></div></div>
      <div class="wd-row"><span>利用日</span><span>${helpers.esc(t.date||'-')}</span></div>
      <div class="wd-row"><span>大人</span><span>${t.adult}名</span></div>
      <div class="wd-row"><span>子ども</span><span>${t.child}名</span></div>
      <div class="wd-row"><span>合計金額</span><span style="color:var(--pri-dk);font-size:18px">¥ ${total.toLocaleString()}</span></div>
    </div>
    <div class="sec-t">支払い方法</div>
    <div class="ml mb4">
      <div class="mi tkpm act" onclick="selGroup('tkpm',this)"><div class="mi-tx">${I.card}Apple Pay</div><div class="radio"></div></div>
      <div class="mi tkpm" onclick="selGroup('tkpm',this)"><div class="mi-tx">${I.card}Visa **** 1234</div><div class="radio"></div></div>
    </div>
    <div class="card" style="background:var(--org-bg);border:1px solid #FFE0B2;box-shadow:none"><p class="ts" style="color:var(--org)">※ これはデモ用の画面です。実際の決済・発券は行われません。</p></div>
    <button class="btn bp mt4" style="padding:16px;font-size:16px" onclick="completeTicket(${total})">購入を確定する (Mock)</button>
  </section>`;
  nav('ticket-confirm');
}
function completeTicket(total){
  const sel=TICKETS.find(x=>x.id===state.ticket.selectedId);
  const ref='TK-'+String(10000+Math.floor(Math.random()*89999));
  setAvatarMood('happy');
  addRecord('tickets',{refNum:ref,ticketName:sel.name,ticketEmoji:sel.em,date:state.ticket.date,adult:state.ticket.adult,child:state.ticket.child,total:total});
  helpers.toast('処理中...');
  setTimeout(()=>{
    $('v-ticket-complete').innerHTML=`<div class="sh"><div style="width:32px"></div><h2>購入完了</h2></div><section class="sec fxc aic" style="padding-top:24px">
      <div class="succ">${I.check}</div>
      <h2 style="font-size:22px;font-weight:800;margin-bottom:8px">購入完了（Mock）</h2>
      <p class="fsub ts mb4 tac">Ticket purchase complete.</p>
      <div class="card w100 tac"><p class="txs fsub mb2">予約番号</p><p style="font-size:22px;font-weight:800;letter-spacing:1px;color:var(--pri-dk)">${ref}</p></div>
      <div class="card w100">
        <div class="wd-row"><span>チケット</span><span>${helpers.esc(sel.name)}</span></div>
        <div class="wd-row"><span>利用日</span><span>${helpers.esc(state.ticket.date||'-')}</span></div>
        <div class="wd-row"><span>大人/子ども</span><span>${state.ticket.adult} / ${state.ticket.child}</span></div>
        <div class="wd-row"><span>支払い金額</span><span style="color:var(--pri-dk);font-size:16px">¥ ${total.toLocaleString()}</span></div>
      </div>
      <button class="btn bp mb3" style="padding:16px;font-size:16px" onclick="nav('home')">ホームへ戻る</button>
      <button class="btn bo" onclick="nav('mobility-hub')">経路・チケットに戻る</button>
    </section>`;
    nav('ticket-complete');
  },700);
}

const bagS={qty:1,size:'中型',factor:1500,dest:'宿泊ホテル',drop:'駅カウンター'};
function renderBaggage(){
  $('v-baggage').innerHTML=helpers.sh('home','手荷物配送')+`<section class="sec">
  <div class="card grad"><div class="fxc aic tac" style="padding:12px 0">${I.bag}<h3 style="font-size:18px;font-weight:800;margin:12px 0 8px">ホテルへ先に送って、<br>身軽に観光</h3><p style="font-size:13px;opacity:.9">大きなスーツケースを持たずに、<br>そのまま日本の街を楽しめます。</p></div></div>
  <button class="btn bp mb4" style="padding:16px;font-size:16px" onclick="renderBagForm();nav('bag-form')">配送を予約する</button>
  <button class="btn bo mb4" style="padding:14px;font-size:14px" onclick="nav('history-baggage')">${I.list} 予約履歴を見る</button>
  <div class="sec-t mt4">代表的な利用シーン</div>
  <div class="ml">${[{l:'空港からホテルへ',s:'到着してすぐ手ぶらで観光へ'},{l:'駅からホテルへ',s:'新幹線を降りたらそのまま街へ'}].map(i=>`<div class="mi" onclick="renderBagForm();nav('bag-form')"><div class="fx aic g3"><div class="gi-icon">${I.send}</div><div class="fxc"><span class="fw7 ts">${i.l}</span><span class="txs fsub">${i.s}</span></div></div>${I.chev}</div>`).join('')}</div></section>`;
}
function renderBagForm(){
  const qOpts=[{v:1,l:'1個'},{v:2,l:'2個'},{v:3,l:'3個以上'}];
  const szOpts=[{v:'small',l:'機内持込',s:'Small',f:1000},{v:'medium',l:'中型',s:'Medium',f:1500},{v:'large',l:'大型',s:'Large',f:2500}];
  const tmOpts=[{v:'now',l:'今すぐ',s:'Now'},{v:'today_pm',l:'今日の午後',s:'PM'},{v:'tomorrow',l:'明日',s:'Tomorrow'}];
  $('v-bag-form').innerHTML=helpers.sh('baggage','配送予約')+`<section class="sec">
  <div class="sec-t">荷物の情報 <small>Details</small></div>
  <p class="ts fw7 mb2">個数</p><div class="sel-grid g3c">${qOpts.map(o=>`<div class="sel-btn bq${o.v===bagS.qty?' act':''}" onclick="bagS.qty=${o.v};selGroup('bq',this)">${o.l}</div>`).join('')}</div>
  <p class="ts fw7 mb2 mt4">サイズ</p><div class="sel-grid g3c">${szOpts.map(o=>`<div class="sel-btn bsz${o.v===bagSizeKey()?' act':''}" onclick="setBagSz('${o.v}',${o.f},'${o.l}');selGroup('bsz',this)">${o.l}<small>${o.s}</small></div>`).join('')}</div>
  <p class="ts fw7 mb2 mt4">預けるタイミング</p><div class="sel-grid g3c" style="margin-bottom:32px">${tmOpts.map((o,i)=>`<div class="sel-btn btm${i===0?' act':''}" onclick="selGroup('btm',this)">${o.l}<small>${o.s}</small></div>`).join('')}</div>
  <div class="sec-t">受取先・預け方</div>
  <p class="ts fw7 mb2">受取先</p>
  <div class="ml mb3"><div class="mi bd act" onclick="bagS.dest='宿泊ホテル';selGroup('bd',this);$('hotelIn').style.display='block'"><div class="mi-tx">${I.home}宿泊ホテル</div><div class="radio"></div></div><div class="mi bd" onclick="bagS.dest='空港';selGroup('bd',this);$('hotelIn').style.display='none'"><div class="mi-tx">${I.plane}空港</div><div class="radio"></div></div></div>
  <div id="hotelIn" style="margin-bottom:24px"><input class="ifield" id="hotelNm" style="width:100%;border:1px solid #E5E5EA" placeholder="ホテル名を入力"></div>
  <p class="ts fw7 mb2">預け方</p>
  <div class="ml" style="margin-bottom:32px">${['駅カウンターで預ける','ホテルフロントで預ける','コンビニで預ける'].map((l,i)=>`<div class="mi bdr${i===0?' act':''}" onclick="bagS.drop='${l}';selGroup('bdr',this)"><div class="mi-tx">${l}</div><div class="radio"></div></div>`).join('')}</div>
  <button class="btn bp" style="padding:16px;font-size:16px" onclick="goBagConf()">確認画面へ進む</button></section>`;
}
function bagSizeKey(){return bagS.size==='中型'?'medium':bagS.size==='機内持込'?'small':'large'}
function setBagSz(k,f,l){bagS.size=l;bagS.factor=f}
function goBagConf(){
  const h=$('hotelNm')?$('hotelNm').value.trim():'';
  bagS.hotel=h;
  const q=bagS.qty>=3?3:bagS.qty, price=bagS.factor*q;
  const qStr=bagS.qty>=3?'3個以上':bagS.qty+'個';
  $('v-bag-confirm').innerHTML=helpers.sh('bag-form','予約確認')+`<section class="sec">
  <div class="card"><div class="fx jcsb aic mb2"><span class="ts fw7 fsub">お預かり</span><span class="fw7">${helpers.esc(bagS.drop)}</span></div><div class="tac fsub" style="margin:8px 0">↓</div><div class="fx jcsb aic"><span class="ts fw7 fsub">お届け先</span><span class="fw7">${helpers.esc(bagS.dest)}</span></div>${bagS.dest==='宿泊ホテル'?`<div class="ts tar mt3" style="color:var(--pri-dk);font-weight:600">${helpers.esc(h)||'(未入力)'}</div>`:''}</div>
  <div class="card fx jcsb aic"><div><div class="ts fw7 fsub mb2">荷物詳細</div><div class="fw7">${helpers.esc(bagS.size)} x ${qStr}</div></div><div class="tar"><div class="ts fw7 fsub mb2">料金目安</div><div class="fw7" style="font-size:20px">¥ ${price.toLocaleString()}</div></div></div>
  <div class="card" style="background:var(--grn-bg);border:1px solid #BDE0FE;box-shadow:none"><div class="fx aic g2 mb2">${I.clock}<span class="fw7">到着予定の目安</span></div><p class="ts fw7">本日 18:00 以降</p></div>
  <button class="btn bp" style="padding:16px;font-size:16px" onclick="helpers.toast('予約を処理中...');setTimeout(()=>{renderBagComplete();nav('bag-complete')},800)">予約を確定する</button></section>`;
  nav('bag-confirm');
}
function renderBagComplete(){
  setAvatarMood('happy');
  const bagRefNum='#BG-'+String(Math.floor(Math.random()*90000)+10000);
  const qStr=bagS.qty>=3?'3個以上':bagS.qty+'個';
  addRecord('baggage',{refNum:bagRefNum,qty:bagS.qty,qtyLabel:qStr,size:bagS.size,dest:bagS.dest,drop:bagS.drop,hotel:bagS.hotel||'',status:'予約済み'});
  $('v-bag-complete').innerHTML=`<div class="sh"><div style="width:32px"></div><h2>予約完了</h2></div><section class="sec fxc aic" style="padding-top:24px">
  <div class="succ">${I.check}</div><h2 style="font-size:22px;font-weight:800;margin-bottom:8px">配送を予約しました</h2><p class="fsub ts mb4 tac">Your delivery is booked.</p>
  <div class="card w100 tac"><p class="txs fsub mb2">予約番号</p><p style="font-size:24px;font-weight:800;letter-spacing:1px;color:var(--pri-dk)">${bagRefNum}</p></div>
  <div class="card w100"><h4 class="ts fw7 mb3">次にやること</h4>${[{n:'1',t:'指定した預け場所でスタッフにこの画面を見せてください。'},{n:'2',t:'ホテルチェックイン時、フロントで荷物を受け取ります。'}].map(s=>`<div class="fx g3 mb3"><div class="step-c">${s.n}</div><p class="ts fsub" style="line-height:1.4">${s.t}</p></div>`).join('')}</div>
  <button class="btn bp mb3" style="padding:16px;font-size:16px" onclick="nav('home')">ホームへ戻る</button>
  <button class="btn bo" style="padding:14px;font-size:14px" onclick="nav('baggage')">もう一件予約する</button></section>`;
}
const tourS={energy:'normal',crowd:'ok',time:'half'};
function renderTour(){
  const ts = state.tourSelections;
  $('v-tour').innerHTML=helpers.sh('home','観光ガイド (Smart Tour)')+`<section class="sec">
  <div class="card grad"><div class="fxc aic tac" style="padding:12px 0">${I.tour}<h3 style="font-size:18px;font-weight:800;margin:12px 0 8px">あなたにぴったりの<br>観光ルートを提案</h3><p style="font-size:13px;opacity:.9">混雑や疲れやすさに合わせて、<br>無理なく回れるプランを作ります。</p></div></div>
  <div class="sec-t mt4">興味・テーマ <small>複数選択可</small></div>
  <div id="tourThemes">${['アート・文化','歴史・寺社','自然・景色','ショッピング','グルメ'].map((t,i)=>`<button class="tchip tour-theme${(ts.themes.length?ts.themes.includes(t):(i===0||i===2))?' act':''}" data-theme="${helpers.esc(t)}" onclick="this.classList.toggle('act')">${t}</button>`).join('')}</div>
  <div class="sec-t mt4">今の体力・コンディション</div>
  <div class="sel-grid g3c">${[{v:'normal',l:'元気',s:'Good'},{v:'tired',l:'少し疲れた',s:'Tired'}].map(o=>`<div class="sel-btn te${o.v===ts.energy?' act':''}" onclick="state.tourSelections.energy='${o.v}';tourS.energy='${o.v}';selGroup('te',this)">${o.l}<small>${o.s}</small></div>`).join('')}</div>
  <div class="sec-t mt4">人混みへの耐性</div>
  <div class="sel-grid">${[{v:'ok',l:'人気スポットOK',s:'Crowds OK'},{v:'avoid',l:'なるべく避けたい',s:'Avoid'}].map(o=>`<div class="sel-btn tc${o.v===ts.crowd?' act':''}" onclick="state.tourSelections.crowd='${o.v}';tourS.crowd='${o.v}';selGroup('tc',this)">${o.l}<small>${o.s}</small></div>`).join('')}</div>
  <div class="sec-t mt4">滞在時間</div>
  <div class="sel-grid g3c">${[{v:'short',l:'1〜2時間',s:'Short'},{v:'half',l:'半日',s:'Half Day'},{v:'full',l:'1日',s:'Full Day'}].map(o=>`<div class="sel-btn tt${o.v===ts.time?' act':''}" onclick="state.tourSelections.time='${o.v}';tourS.time='${o.v}';selGroup('tt',this)">${o.l}<small>${o.s}</small></div>`).join('')}</div>
  <div class="sec-t mt4">こだわり・希望 <small>自由入力 (任意)</small></div>
  <textarea class="tour-free-text" id="tourFreeText" placeholder="例：静かな場所を中心に回りたい / 子ども連れなので休憩しやすい場所がよい / 和の雰囲気を感じたい、写真映えする場所に行きたい" maxlength="500">${helpers.esc(ts.freeText||'')}</textarea>
  <button class="btn bp" style="padding:16px;font-size:16px" onclick="startTourAI()">AIにおすすめを作ってもらう</button>
  <button class="btn bo mt3" style="padding:14px;font-size:14px" onclick="nav('history-tours')">${I.list} 保存した旅行プランを見る</button></section>`;
}

/* === Fallback tour plans (used only when AI fails) === */
const tourPlans={
  relax:{title:'静寂の庭園とアート巡り',crowd:'少',crowdCls:'b-grn',rest:'しやすい',restCls:'b-blu',time:'約3時間',spots:'根津美術館 → 庭園カフェ → 日本庭園',note:'人混みを避けた美術館と庭園の組み合わせ。'},
  classic:{title:'東京の王道スポット満喫',crowd:'多',crowdCls:'b-red',rest:'普通',restCls:'badge',time:'約4時間',spots:'浅草寺 → 仲見世通り → スカイツリー',note:'見どころが詰まった定番プラン。'},
  short:{title:'絶景サクッと観光',crowd:'中',crowdCls:'b-org',rest:'しやすい',restCls:'b-blu',time:'約1.5時間',spots:'展望台 → 屋内カフェラウンジ',note:'短時間で満足度の高いコンパクトルート。'}
};
function tourOrder(){
  if(tourS.time==='short')return['short','relax','classic'];
  if(tourS.crowd==='avoid'||tourS.energy==='tired')return['relax','short','classic'];
  return['classic','relax','short'];
}

/* === AI Tour Guide Functions === */
function collectTourSelections(){
  const themes = Array.from(document.querySelectorAll('.tour-theme.act')).map(e=>e.dataset.theme);
  const freeText = ($('tourFreeText')?.value||'').trim();
  state.tourSelections.themes = themes;
  state.tourSelections.freeText = freeText;
  state.tourSelections.energy = tourS.energy;
  state.tourSelections.crowd = tourS.crowd;
  state.tourSelections.time = tourS.time;
  return state.tourSelections;
}

function buildTourPrompt(){
  const sel = collectTourSelections();
  const p = state.profile||{};
  const L = state.location;
  const loc = (L.permission==='granted'&&L.label)?L.label:(L.fallback||'東京');
  const w = state.weather?.current;
  const spots = state.nearbySpots.slice(0,5).map(s=>s.name).join(', ');
  const now = new Date();
  const timeLabel = {short:'1〜2時間',half:'半日',full:'1日'}[sel.time]||sel.time;
  const energyLabel = sel.energy==='tired'?'少し疲れている':'元気';
  const crowdLabel = sel.crowd==='avoid'?'人混みを避けたい':'人気スポットOK';

  return `あなたは日本の観光ガイドAIです。以下の情報に基づき、ユーザーに最適な観光プランを3件作成してください。

## ユーザー情報
- 氏名: ${p.name||'ゲスト'}
- 国籍: ${p.nationality||'不明'}
- 使用言語: ${(p.languages||[]).join(', ')||'日本語'}
- 年齢: ${p.age||'不明'}
- 性別: ${p.gender||'不明'}
- 趣味嗜好: ${(p.preferences||[]).join(', ')||'不明'}
- 日本訪問回数: ${p.japanVisitCount||'不明'}

## 観光条件
- 現在地/基準位置: ${loc}
- 興味・テーマ: ${sel.themes.length?sel.themes.join(', '):'特になし'}
- 体力: ${energyLabel}
- 人混み耐性: ${crowdLabel}
- 滞在時間: ${timeLabel}
${sel.freeText?`- ユーザーの希望（自由記述）: ${sel.freeText}`:''}

## 周辺情報
${w?`- 天気: ${helpers.mapWeatherToIcon(w.code).label} ${w.temp}℃`:'- 天気: 不明'}
- 現在時刻: ${now.getHours()}:${String(now.getMinutes()).padStart(2,'0')}
${spots?`- 近隣スポット: ${spots}`:''}

## 出力ルール
必ず以下のJSON形式のみで返してください。コードブロック(\`\`\`)は不要です。JSONのみ出力してください。
{
  "intro": "ユーザー向けの総評コメント（2〜3文）",
  "plans": [
    {
      "id": "plan_1",
      "title": "プラン名",
      "summary": "一言要約",
      "reason_for_you": "なぜこのユーザーに合うのか（2〜3文）",
      "duration": "所要時間",
      "walking_load": "歩行量（少なめ/普通/多め）",
      "crowd_level": "混雑レベル（少/中/多）",
      "rest_level": "休憩しやすさ（しやすい/普通/しにくい）",
      "best_time": "おすすめ時間帯",
      "main_spots": ["スポット1","スポット2","スポット3"],
      "route_steps": ["ステップ1","ステップ2","ステップ3"],
      "rest_spots": ["休憩候補1","休憩候補2"],
      "tips": ["補足1","補足2"]
    }
  ]
}
- plansは3件。1件目は最もおすすめ、2件目は代替案、3件目は別方向の提案。
- 各プランはユーザー属性・趣向・自由記述に基づき差別化すること。
- スポット名は実在する場所を使うこと。`;
}

/* ===== Fetch with Retry (for 503 / 429 transient errors) ===== */
async function fetchWithRetry(url, options, maxRetries=2){
  for(let attempt=0; attempt<=maxRetries; attempt++){
    const response = await fetch(url, options);
    if(response.ok) return response;
    if((response.status===503||response.status===429) && attempt<maxRetries){
      const wait = (attempt+1)*2000; /* 2s, 4s */
      console.warn(`API ${response.status}, retrying in ${wait}ms (attempt ${attempt+1}/${maxRetries})...`);
      await new Promise(r=>setTimeout(r, wait));
      continue;
    }
    /* Non-retryable error or max retries exceeded */
    const errBody = await response.text().catch(()=>'');
    console.error(`API error ${response.status}:`, errBody);
    throw new Error(`API ${response.status}`);
  }
}

async function callTourGuideAI(){
  const provider = getAdminSetting('aiProvider','claude');
  const tourPrompt = buildTourPrompt();
  /* 観光ガイド専用のシステムプロンプト (管理者設定のチャット用プロンプトとは分離) */
  const tourSysPrompt = 'あなたは日本の観光ガイドAIです。ユーザーのリクエストに従い、指定されたJSON形式のみで回答してください。コードブロックや説明文は不要です。JSONオブジェクトのみ出力してください。';

  try{
    let text = '';

    if(provider === 'openai'){
      const apiKey = getAdminSetting('openAiApiKey','');
      if(!apiKey) throw new Error('OpenAI APIキーが未設定です。管理者設定から設定してください。');
      const msgs = [{role:'system',content:tourSysPrompt},{role:'user',content:tourPrompt}];
      const response = await fetchWithRetry('https://api.openai.com/v1/chat/completions',{
        method:'POST',
        headers:{'Content-Type':'application/json','Authorization':'Bearer '+apiKey},
        body:JSON.stringify({model:'gpt-4o-mini',max_tokens:4096,messages:msgs})
      });
      const data = await response.json();
      text = data.choices?.[0]?.message?.content || '';

    }else if(provider === 'gemini'){
      const apiKey = getAdminSetting('geminiApiKey','');
      if(!apiKey) throw new Error('Gemini APIキーが未設定です。管理者設定から設定してください。');
      const contents = [{role:'user',parts:[{text:tourPrompt}]}];
      const response = await fetchWithRetry(`https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key=${apiKey}`,{
        method:'POST',
        headers:{'Content-Type':'application/json'},
        body:JSON.stringify({
          system_instruction:{parts:[{text:tourSysPrompt}]},
          contents:contents,
          generationConfig:{
            maxOutputTokens:4096,
            responseMimeType:'application/json',
            thinkingConfig:{thinkingBudget:0}
          }
        })
      });
      const data = await response.json();
      text = (data.candidates?.[0]?.content?.parts||[]).filter(p=>!p.thought).map(p=>p.text).filter(Boolean).join('\n') || '';

    }else{
      const apiKey = getAdminSetting('claudeApiKey','');
      if(!apiKey) throw new Error('Claude APIキーが未設定です。管理者設定から設定してください。');
      const response = await fetchWithRetry('https://api.anthropic.com/v1/messages',{
        method:'POST',
        headers:{'Content-Type':'application/json','x-api-key':apiKey,'anthropic-version':'2023-06-01','anthropic-dangerous-direct-browser-access':'true'},
        body:JSON.stringify({model:'claude-sonnet-4-20250514',max_tokens:4096,system:tourSysPrompt,messages:[{role:'user',content:tourPrompt}]})
      });
      const data = await response.json();
      text = data.content.filter(b=>b.type==='text').map(b=>b.text).join('\n');
    }
    return text;
  }catch(e){ throw e; }
}

function parseTourGuideResponse(raw){
  if(!raw || typeof raw !== 'string') return null;
  /* Strategy 1: Direct parse */
  try{
    const direct = JSON.parse(raw.trim());
    if(direct && Array.isArray(direct.plans) && direct.plans.length>0) return direct;
  }catch(e){}

  /* Strategy 2: Strip markdown code fences (```json ... ```) */
  try{
    const fenceMatch = raw.match(/```(?:json)?\s*\n?([\s\S]*?)\n?\s*```/i);
    if(fenceMatch){
      const parsed = JSON.parse(fenceMatch[1].trim());
      if(parsed && Array.isArray(parsed.plans) && parsed.plans.length>0) return parsed;
    }
  }catch(e){}

  /* Strategy 3: Find first { and last } to extract JSON object */
  try{
    const firstBrace = raw.indexOf('{');
    const lastBrace = raw.lastIndexOf('}');
    if(firstBrace !== -1 && lastBrace > firstBrace){
      const extracted = raw.substring(firstBrace, lastBrace + 1);
      const parsed = JSON.parse(extracted);
      if(parsed && Array.isArray(parsed.plans) && parsed.plans.length>0) return parsed;
    }
  }catch(e){}

  console.error('Tour JSON parse failed. Raw response:', raw.substring(0, 500));
  return null;
}

async function startTourAI(){
  setAvatarMood('thinking');
  collectTourSelections();
  /* Show loading */
  $('v-tour-results').innerHTML=helpers.sh('tour','提案プラン')+`<section class="sec"><div class="tour-loading"><div class="tl-spinner"></div><div class="tl-msg">AIがあなた専用のプランを作成中...</div><div class="tl-sub">条件・プロフィール・天気を分析しています</div></div></section>`;
  nav('tour-results');

  try{
    const raw = await callTourGuideAI();
    const parsed = parseTourGuideResponse(raw);
    if(parsed){
      state.generatedTourPlans = parsed;
      /* Save tour to history */
      setAvatarMood('happy');
      addRecord('tours',{conditions:{...state.tourSelections},plans:parsed.plans,intro:parsed.intro||'',location:services.resolveCoords().label});
      renderTourResultsAI(parsed);
    }else{
      /* Fallback to fixed plans */
      helpers.toast('AI応答の解析に失敗しました。おすすめプランを表示します。');
      renderTourResultsFallback();
    }
  }catch(e){
    console.error('Tour AI error:',e);
    helpers.toast('エラー: '+e.message);
    renderTourResultsFallback();
  }
}

function crowdBadgeClass(level){
  if(!level) return 'b-org';
  if(/少|low|quiet/i.test(level)) return 'b-grn';
  if(/多|high|busy|crowded/i.test(level)) return 'b-red';
  return 'b-org';
}
function restBadgeClass(level){
  if(!level) return 'b-blu';
  if(/しやすい|easy|good/i.test(level)) return 'b-blu';
  if(/しにくい|hard|difficult/i.test(level)) return 'b-org';
  return 'badge';
}

function renderTourResultsAI(data){
  let html=helpers.sh('tour','提案プラン')+'<section class="sec">';
  if(data.intro){
    html+=`<div class="card" style="background:#F0F8FF;border:1px solid #BDE0FE;box-shadow:none"><p class="ts fw7 mb2 fx aic g2">${I.star} AIコメント</p><p class="ts" style="color:var(--pri-dk)">${helpers.esc(data.intro)}</p></div>`;
  }
  (data.plans||[]).forEach((plan,i)=>{
    const isTop = i===0;
    const spots = Array.isArray(plan.main_spots)?plan.main_spots.join(' → '):(plan.main_spots||'');
    html+=`<div class="tour-ai-card${isTop?' top':''}" onclick="openTourDetailAI(${i})">
      <div class="tac-head"><span class="em">${isTop?'⭐':'📍'}</span><span class="l">${helpers.esc(plan.title||'プラン'+(i+1))}</span>${isTop?'<span class="badge b-blu" style="font-size:10px">AIおすすめ</span>':''}</div>
      ${plan.reason_for_you?`<div class="tac-reason">💡 ${helpers.esc(plan.reason_for_you)}</div>`:''}
      <div class="tac-meta">
        <span class="badge ${crowdBadgeClass(plan.crowd_level)}">混雑: ${helpers.esc(plan.crowd_level||'-')}</span>
        <span class="badge ${restBadgeClass(plan.rest_level)}">休憩: ${helpers.esc(plan.rest_level||'-')}</span>
        ${plan.duration?`<span class="badge b-blu">所要: ${helpers.esc(plan.duration)}</span>`:''}
      </div>
      <div class="tac-spots">${helpers.esc(spots)}</div>
      ${plan.summary?`<p class="ts fsub mt3">${helpers.esc(plan.summary)}</p>`:''}
    </div>`;
  });
  html+='</section>';
  $('v-tour-results').innerHTML=html;
}

function openTourDetailAI(idx){
  const data = state.generatedTourPlans;
  if(!data||!data.plans||!data.plans[idx]){ helpers.toast('プランデータが見つかりません'); return; }
  const plan = data.plans[idx];
  state.selectedTourPlan = plan;
  const spots = Array.isArray(plan.main_spots)?plan.main_spots:[];
  const steps = Array.isArray(plan.route_steps)?plan.route_steps:[];
  const rests = Array.isArray(plan.rest_spots)?plan.rest_spots:[];
  const tips = Array.isArray(plan.tips)?plan.tips:[];

  let html = helpers.sh('tour-results','プラン詳細')+`<section class="sec">
  <div class="card">
    <h3 style="font-size:20px;font-weight:800;margin-bottom:8px">${helpers.esc(plan.title||'')}</h3>
    ${plan.summary?`<p class="ts fsub mb3">${helpers.esc(plan.summary)}</p>`:''}
    <div class="fx g2" style="flex-wrap:wrap;margin-bottom:12px">
      <span class="badge ${crowdBadgeClass(plan.crowd_level)}">混雑: ${helpers.esc(plan.crowd_level||'-')}</span>
      <span class="badge ${restBadgeClass(plan.rest_level)}">休憩: ${helpers.esc(plan.rest_level||'-')}</span>
      ${plan.duration?`<span class="badge b-blu">所要: ${helpers.esc(plan.duration)}</span>`:''}
      ${plan.walking_load?`<span class="badge b-org">歩行: ${helpers.esc(plan.walking_load)}</span>`:''}
      ${plan.best_time?`<span class="badge b-grn">推奨: ${helpers.esc(plan.best_time)}</span>`:''}
    </div>
  </div>`;

  if(plan.reason_for_you){
    html+=`<div class="card" style="background:#F0F8FF;border:1px solid #BDE0FE;box-shadow:none">
      <p class="ts fw7 mb2" style="color:var(--pri-dk)">💡 なぜあなた向けか</p>
      <p class="ts" style="line-height:1.6">${helpers.esc(plan.reason_for_you)}</p>
    </div>`;
  }

  if(spots.length){
    html+=`<div class="card flat"><p class="ts fw7 mb3">🗺️ 主なスポット</p>
      <p class="ts">${helpers.esc(spots.join(' → '))}</p>
    </div>`;
  }

  if(steps.length){
    html+=`<div class="card flat"><p class="ts fw7 mb3">🚶 回遊ステップ</p>
      ${steps.map((s,i)=>`<div class="fx g3 mb3"><div class="step-c">${i+1}</div><p class="ts" style="line-height:1.5">${helpers.esc(s)}</p></div>`).join('')}
    </div>`;
  }

  if(rests.length){
    html+=`<div class="card flat"><p class="ts fw7 mb3">☕ 休憩候補</p>
      ${rests.map(r=>`<div class="fx aic g2 mb2"><span style="color:var(--grn)">●</span><span class="ts">${helpers.esc(r)}</span></div>`).join('')}
    </div>`;
  }

  if(tips.length){
    html+=`<div class="card flat" style="background:#FFFBF2"><p class="ts fw7 mb3">📝 注意点・ヒント</p>
      ${tips.map(t=>`<div class="fx aic g2 mb2"><span style="color:var(--org)">●</span><span class="ts">${helpers.esc(t)}</span></div>`).join('')}
    </div>`;
  }

  html+=`<div class="card" style="background:#F2F2F7;box-shadow:none"><p class="ts fw7 mb3">このプランに便利な機能</p>
    <button class="btn ts mb2" style="padding:14px;background:#fff;border:1px solid #E5E5EA" onclick="state.mobility.destination='${helpers.esc((spots[0]||plan.title||'').split(' ')[0])}';saveState();nav('mobility');renderMobility()">🚋 目的地までの経路を開く</button>
    <button class="btn ts" style="padding:14px;background:#fff;border:1px solid #E5E5EA" onclick="nav('baggage')">🧳 荷物を先に送って身軽になる</button>
  </div></section>`;

  $('v-tour-detail').innerHTML=html;
  nav('tour-detail');
}

/* === Fallback rendering (uses fixed tourPlans when AI fails) === */
function renderTourResultsFallback(){
  const order=tourOrder();
  let comment='人気スポットを中心に効率よく回れるプランを作成しました。';
  if(tourS.crowd==='avoid'||tourS.energy==='tired')comment='人混みを避け、ゆったり回れるルートを優先しました。';
  else if(tourS.time==='short')comment='短時間でサクッと楽しめるプランを作成しました。';
  let html=helpers.sh('tour','提案プラン')+'<section class="sec">';
  html+=`<div class="card" style="background:var(--org-bg);border:1px solid #FFE0B2;box-shadow:none"><p class="ts fw7 mb2" style="color:var(--org)">⚠ AI生成に失敗したため、おすすめプランを表示しています</p></div>`;
  html+=`<div class="card" style="background:#F0F8FF;border:1px solid #BDE0FE;box-shadow:none"><p class="ts fw7 mb2 fx aic g2">${I.star} AIコメント</p><p class="ts" style="color:var(--pri-dk)">${comment}</p></div>`;
  order.forEach((k,i)=>{
    const p=tourPlans[k];
    html+=`<div class="rc" onclick="openTourDetailFallback('${k}')">
      <div class="rc-hd"><span class="em">${i===0?'⭐':'📍'}</span><span class="l">${p.title}</span></div>
      <div class="fx g2 mb2"><span class="badge ${p.crowdCls}">混雑: ${p.crowd}</span><span class="badge ${p.restCls}">休憩: ${p.rest}</span></div>
      <div class="rc-sub">所要: ${p.time} ・ ${p.spots}</div>
    </div>`;
  });
  html+='</section>';
  $('v-tour-results').innerHTML=html;
}

function openTourDetailFallback(k){
  const p=tourPlans[k];
  $('v-tour-detail').innerHTML=helpers.sh('tour-results','プラン詳細')+`<section class="sec">
  <div class="card"><h3 style="font-size:20px;font-weight:800;margin-bottom:8px">${p.title}</h3>
  <div class="fx g2 mb3"><span class="badge ${p.crowdCls}">混雑: ${p.crowd}</span><span class="badge ${p.restCls}">休憩: ${p.rest}</span></div>
  <p class="ts fw7 fsub mb3">所要: ${p.time}</p>
  <div style="background:#F0F8FF;padding:12px;border-radius:8px;font-size:13px;color:var(--pri-dk);line-height:1.5">💡 AI提案の理由<br><span style="color:var(--tx)">${p.note}</span></div></div>
  <div class="card flat"><p class="ts fw7 mb2">主な行き先</p><p class="ts">${p.spots}</p></div>
  <div class="card" style="background:#F2F2F7;box-shadow:none"><p class="ts fw7 mb3">このプランに便利な機能</p>
    <button class="btn ts mb2" style="padding:14px;background:#fff;border:1px solid #E5E5EA" onclick="state.mobility.destination='${p.title.split(' ')[0]}';saveState();nav('mobility');renderMobility()">🚋 目的地までの経路を開く</button>
    <button class="btn ts" style="padding:14px;background:#fff;border:1px solid #E5E5EA" onclick="nav('baggage')">🧳 荷物を先に送って身軽になる</button>
  </div></section>`;
  nav('tour-detail');
}
/* === End Tour Guide === */
const troubleData={
  health:{title:'体調不良・ケガ',color:'var(--org)',bg:'var(--org-bg)',tag:'Health',
    steps:['安全な場所で座り、安静にしてください。','水分を補給し、症状を確認してください。','<span style="color:var(--red);font-weight:700">※呼吸困難・激しい痛み・意識障害がある場合はすぐ119へ</span>'],
    places:[{n:'〇〇インターナショナルクリニック',s:'英語対応 / 内科・外科',d:'徒歩5分'},{n:'△△薬局',s:'市販薬・処方箋',d:'徒歩2分'}],
    contacts:'ホテルフロント（救急車手配可）',insurance:'提携病院かどうか保険会社に確認。領収書・診断書は必ず保管。',ai:'体調が悪いです。近くの受診先を知りたいです。'},
  disaster:{title:'災害・避難',color:'var(--red)',bg:'var(--red-bg)',tag:'Disaster',
    steps:['身の安全を確保。（頭を守り、落下物から離れる）','揺れが収まるまで待機。慌てて屋外に出ない。','落ち着いたら交通機関の運行状況や避難指示を確認。'],
    places:[{n:'××小学校 (一時避難場所)',s:'広域避難所',d:'徒歩8分'},{n:'新宿駅 観光案内所',s:'多言語支援',d:'徒歩10分'}],
    contacts:'自国の大使館・領事館 / 宿泊先ホテル',insurance:'災害による追加宿泊費や航空券変更費用が補償されるか確認。',ai:'災害時の安全な行動を教えてください。'},
  lost:{title:'遺失物・落とし物',color:'var(--pri)',bg:'#F0F8FF',tag:'Lost Item',
    steps:['無くした場所と時間を落ち着いて整理。','直近の立ち寄り先に電話確認。','カード・スマホは停止手続きを。'],
    places:[{n:'交番 (Police Box)',s:'遺失物届の提出',d:'徒歩3分'},{n:'JR お忘れ物承り所',s:'駅での落とし物検索',d:'駅構内'}],
    contacts:'クレジットカード会社 / タクシー・鉄道コールセンター',insurance:'携行品損害の確認。警察で遺失物届の受理番号をもらう。',ai:'財布をなくしました。どう動けばよいですか？'}
};
function renderTrouble(){
  setAvatarMood('alert');
  $('v-trouble').innerHTML=helpers.sh('home','トラブル・SOS')+`<section class="sec">
  <div style="background:var(--red);color:#fff;border-radius:var(--r-sm);padding:24px 16px;margin-bottom:32px;text-align:center">
    ${I.sos}<h3 style="font-weight:800;font-size:18px;margin:12px 0 6px">命の危険がある場合</h3><p style="font-size:13px;font-weight:600;opacity:.95">すぐに以下の番号へ連絡してください。</p>
    <div class="fx g2" style="margin-top:20px">${[{n:'119',l:'救急・消防',e:'🚑'},{n:'110',l:'警察',e:'🚓'}].map(c=>`<button class="btn" style="background:#fff;color:var(--red);flex:1;font-weight:800;font-size:16px;border-radius:8px;padding:12px" onclick="helpers.toast('${c.n}に発信します (Mock)')">${c.e} ${c.n}<br><span style="font-size:11px;font-weight:600;color:var(--txs)">${c.l}</span></button>`).join('')}</div>
  </div>
  <div class="sec-t">状況から探す <small>Select Category</small></div>
  <div class="ml">${Object.entries(troubleData).map(([k,v])=>`<div class="mi" onclick="openTroubleDetail('${k}')"><div class="fx aic g3"><div class="gi-icon" style="background:${v.bg};color:${v.color};border-radius:50%">${k==='health'?I.health:k==='disaster'?I.sos:I.search}</div><div class="fxc"><span style="font-size:15px;font-weight:700">${v.title}</span></div></div>${I.chev}</div>`).join('')}</div></section>`;
}
function openTroubleDetail(k){
  const d=troubleData[k];
  $('v-trouble-detail').innerHTML=helpers.sh('trouble','対応ガイド')+`<section class="sec">
  <div class="card" style="border-top:4px solid ${d.color};border-radius:8px"><div class="fx jcsb aic mb3"><h3 style="font-size:20px;font-weight:800">${d.title}</h3><span class="badge" style="background:${d.bg};color:${d.color}">${d.tag}</span></div><h4 class="ts fw7 mb2">1. まずやること</h4><ul style="font-size:13px;color:var(--txs);margin-left:20px;line-height:1.6;margin-bottom:16px">${d.steps.map(s=>`<li style="margin-bottom:8px">${s}</li>`).join('')}</ul></div>
  <div class="card flat"><h4 class="ts fw7 mb3 fx aic g2">${I.pin} 近くの施設</h4>${d.places.map(p=>`<div class="fx jcsb aic" style="padding:6px 0"><div><div class="fw7 ts">${p.n}</div><div class="txs fsub">${p.s}</div></div><div class="txs fw7" style="color:var(--pri)">${p.d}</div></div>`).join('')}</div>
  <div class="card flat"><h4 class="ts fw7 mb3 fx aic g2">${I.phone} 連絡先</h4><p class="ts">${d.contacts}</p></div>
  <div class="card flat" style="background:#F9F9F9"><h4 class="ts fw7 mb3 fx aic g2">${I.shield} 保険・補償</h4><p class="ts fsub">${d.insurance}</p></div>
  <button class="btn bp mb4" style="padding:16px;font-size:16px" onclick="openChat('${d.ai}')"><span class="fx aic jcsb" style="justify-content:center;gap:8px"><span style="display:inline-flex;width:24px;height:24px">${charaSVG(24)}</span>AIに相談する</span></button></section>`;
  nav('trouble-detail');
}
const rfItems=[
  {id:1,shop:'マツモトキヨシ 新宿東口店',date:'2026/04/12',cat:'消耗品',amt:12500,ok:false},
  {id:2,shop:'ドン・キホーテ 浅草店',date:'2026/04/13',cat:'消耗品',amt:8300,ok:false},
  {id:3,shop:'ヨドバシカメラ 秋葉原店',date:'2026/04/14',cat:'一般物品',amt:27200,ok:true}
];
function renderRefund(){
  const okC=rfItems.filter(i=>i.ok).length, ngC=rfItems.length-okC;
  $('v-refund').innerHTML=helpers.sh('home','免税リファンド')+`<section class="sec">
  <div class="card grad" style="padding:20px 16px"><div class="fxc aic tac">${I.yen}<h3 style="font-size:18px;font-weight:800;margin:12px 0 8px">購入情報をまとめて、<br>出国前の免税手続きを簡単に</h3></div></div>
  <div class="card flat"><p class="ts fw7 fsub mb2">現在の進捗</p><div class="fx jcsb" style="align-items:flex-end"><div><span class="fw7" style="font-size:28px">${rfItems.length}</span><span class="ts fsub" style="margin-left:4px">件の購入</span></div><div class="fxc" style="align-items:flex-end;gap:4px"><span class="badge b-grn">準備OK: ${okC}件</span><span class="badge b-org">未確認: ${ngC}件</span></div></div></div>
  <button class="btn bp mb4" style="padding:16px;font-size:16px" onclick="renderRefundForm();nav('refund-form')">購入情報を整理する</button>
  <div class="sec-t mt4">出国前チェック <small>Checklist</small></div>
  <div class="card flat">${['パスポートを持っている','購入した免税品が手元にある','すべてのレシート・購入記録が揃っている'].map(t=>`<div class="fx aic g3 mb3"><input type="checkbox" class="ckb"><span class="ts fw7">${t}</span></div>`).join('')}</div></section>`;
}
function renderRefundForm(){
  $('v-refund-form').innerHTML=helpers.sh('refund','購入情報の一覧')+`<section class="sec">
  <div class="sec-t">免税対象の購入 <small>Purchases</small></div>
  ${rfItems.map(i=>`<div class="card mb3"><div class="fx jcsb" style="align-items:flex-start;margin-bottom:12px"><div><div class="fw7 ts">${i.shop}</div><div class="txs fsub">${i.date} • ${i.cat}</div></div><div class="fw7">¥ ${i.amt.toLocaleString()}</div></div><div class="fx jcsb aic" style="border-top:1px dashed #E5E5EA;padding-top:12px"><span class="badge ${i.ok?'b-grn':'b-org'}" id="rfs${i.id}">${i.ok?'準備OK':'未確認'}</span><button class="btn txs" style="padding:8px 16px;background:${i.ok?'#F2F2F7':'#F0F8FF'};color:${i.ok?'var(--txs)':'var(--pri)'};width:auto" onclick="togRf(${i.id},this)">${i.ok?'未確認に戻す':'確認済みにする'}</button></div></div>`).join('')}
  <button class="btn bo mb4" style="border:2px dashed var(--pri);font-size:14px" onclick="helpers.toast('レシート読み取り (Mock)')">＋ レシートを読み取って追加</button>
  <button class="btn bp" style="padding:16px;font-size:16px" onclick="renderRefundConfirm();nav('refund-confirm')">申請確認へ進む</button></section>`;
}
function togRf(id,btn){
  const it=rfItems.find(i=>i.id===id); it.ok=!it.ok;
  const b=$('rfs'+id);
  b.textContent=it.ok?'準備OK':'未確認'; b.className='badge '+(it.ok?'b-grn':'b-org');
  btn.textContent=it.ok?'未確認に戻す':'確認済みにする'; btn.style.background=it.ok?'#F2F2F7':'#F0F8FF'; btn.style.color=it.ok?'var(--txs)':'var(--pri)';
  renderTodoList();
}
function renderRefundConfirm(){
  const total=rfItems.reduce((s,i)=>s+i.amt,0); const refAmt=Math.round(total*0.1);
  $('v-refund-confirm').innerHTML=helpers.sh('refund-form','申請確認')+`<section class="sec">
  <div class="card"><div class="fx jcsb aic mb2"><span class="ts fw7 fsub">対象件数</span><span class="fw7">${rfItems.length} 件</span></div><div class="fx jcsb aic mb2"><span class="ts fw7 fsub">購入総額</span><span class="fw7">¥ ${total.toLocaleString()}</span></div><div class="fx jcsb aic" style="border-top:1px solid #E5E5EA;padding-top:12px;margin-top:12px"><span class="ts fw7" style="color:var(--pri-dk)">還付予定額の目安</span><span class="fw7" style="color:var(--pri);font-size:20px">約 ¥ ${refAmt.toLocaleString()}</span></div></div>
  <div class="sec-t">返金方法</div>
  <div class="ml mb4"><div class="mi rfm act" onclick="selGroup('rfm',this)"><div class="mi-tx">${I.card}クレジットカードへ返金</div><div class="radio"></div></div><div class="mi rfm" onclick="selGroup('rfm',this)"><div class="mi-tx">${I.yen}空港窓口で現金受取</div><div class="radio"></div></div></div>
  <div class="card" style="background:var(--red-bg);border:1px solid #FFC6C4;box-shadow:none;padding:12px"><p class="ts fw7" style="color:var(--red);line-height:1.5">店舗ごとに対応が異なる場合があります。出国前に空港の税関で最終手続きが必要です。</p></div>
  <button class="btn bp mt4" style="padding:16px;font-size:16px" onclick="helpers.toast('処理中...');setTimeout(()=>{renderRefundComplete(${refAmt});nav('refund-complete')},800)">申請準備を完了する</button></section>`;
}
function renderRefundComplete(amt){
  const total=rfItems.reduce((s,i)=>s+i.amt,0);
  addRecord('refunds',{total:total,refundAmt:amt,itemCount:rfItems.length,items:rfItems.map(i=>({shop:i.shop,date:i.date,amt:i.amt,cat:i.cat}))});
  $('v-refund-complete').innerHTML=`<div class="sh"><div style="width:32px"></div><h2>準備完了</h2></div><section class="sec fxc aic" style="padding-top:24px">
  <div class="succ">${I.check}</div><h2 style="font-size:22px;font-weight:800;margin-bottom:8px">申請準備が完了しました</h2><p class="fsub ts mb4 tac">Tax-free preparation complete.</p>
  <div class="card w100 tac"><p class="txs fsub mb2">還付予定額</p><p style="font-size:28px;font-weight:800;color:var(--pri)">¥ ${amt.toLocaleString()}</p></div>
  <div class="card w100"><h4 class="ts fw7 mb3">次にやること</h4>${[{n:'1',t:'未処理の購入がある場合は追加確認を。'},{n:'2',t:'出国時、空港の税関でパスポートと免税品を提示。'}].map(s=>`<div class="fx g3 mb3"><div class="step-c">${s.n}</div><p class="ts fsub" style="line-height:1.4">${s.t}</p></div>`).join('')}</div>
  <button class="btn bp mb3" style="padding:16px;font-size:16px" onclick="nav('home')">ホームへ戻る</button>
  <button class="btn bo" style="padding:14px;font-size:14px" onclick="nav('refund')">もう一度確認する</button></section>`;
}
const oacS={airline:'',flight:'',airport:'',date:'',time:'',ref:'',bags:0,counter:'tokyo',counterName:'東京駅 八重洲カウンター',slot:'10:00-10:30',elig:'',saved:90,refNum:''};
function renderOac(){
  $('v-oac').innerHTML=helpers.sh('home','空港外チェックイン')+`<section class="sec">
  <div class="oac-hero"><div style="width:56px;height:56px;border-radius:16px;background:rgba(255,255,255,.15);display:flex;align-items:center;justify-content:center;margin-bottom:16px">${I.plane}</div><h3>駅で先にチェックインして、<br>最後まで旅行を楽しむ</h3><p>空港での長い待ち時間を減らし、<br>出発ギリギリまで日本を満喫できます。</p></div>
  <div class="oac-ts"><div class="oac-ts-i">${I.clock}</div><div><h4>最大90分の余裕</h4><p>通常より空港到着を遅らせられる可能性があります。</p></div></div>
  <button class="btn bp mb4" style="padding:16px;font-size:16px" onclick="renderOacForm();nav('oac-form')">フライト情報を入力して利用可否を確認</button>
  <div class="card" style="background:#F2F2F7;box-shadow:none"><h4 class="ts fw7 mb2">ご利用について</h4><div class="fx g2 mb2" style="align-items:flex-start">${I.info}<p class="txs fsub" style="line-height:1.5">対応可否は航空会社・便・時間帯によって異なります。</p></div><div class="fx g2" style="align-items:flex-start">${I.info}<p class="txs fsub" style="line-height:1.5">預け荷物がある場合、条件が異なることがあります。</p></div></div></section>`;
}
function renderOacForm(){
  const tomorrow=new Date(); tomorrow.setDate(tomorrow.getDate()+1);
  const defDate=tomorrow.toISOString().split('T')[0];
  const airlines=['ANA (全日空)','JAL (日本航空)','United Airlines','Delta Air Lines','Korean Air','その他'];
  const airports=[{v:'NRT',l:'成田国際空港 (NRT)'},{v:'HND',l:'羽田空港 (HND)'},{v:'KIX',l:'関西国際空港 (KIX)'}];
  const times=['09:00','10:00','11:00','12:00','13:00','14:00','15:00','16:00','17:00','18:00','19:00','20:00','21:00'];
  $('v-oac-form').innerHTML=helpers.sh('oac','フライト情報入力')+`<section class="sec">
  <div class="sec-t">フライト情報 <small>Flight Details</small></div>
  <div class="sbox">
    <div class="irow"><div class="ii">${I.plane}</div><select id="oacAl" class="ifield" style="appearance:auto"><option value="">航空会社を選択</option>${airlines.map(a=>`<option value="${a}">${a}</option>`).join('')}</select></div><div class="divider"></div>
    <div class="irow"><div class="ii">${I.flag}</div><input class="ifield" id="oacFn" placeholder="便名 (例: NH101)"></div><div class="divider"></div>
    <div class="irow"><div class="ii">${I.pin}</div><select id="oacAp" class="ifield" style="appearance:auto"><option value="">出発空港を選択</option>${airports.map(a=>`<option value="${a.v}">${a.l}</option>`).join('')}</select></div><div class="divider"></div>
    <div class="irow"><div class="ii">${I.cal}</div><input type="date" id="oacDt" class="ifield" value="${defDate}"></div><div class="divider"></div>
    <div class="irow"><div class="ii">${I.clock}</div><select id="oacTm" class="ifield" style="appearance:auto"><option value="">出発時刻を選択</option>${times.map(t=>`<option value="${t}">${t}</option>`).join('')}</select></div><div class="divider"></div>
    <div class="irow"><div class="ii">${I.lock}</div><input class="ifield" id="oacRef" placeholder="予約番号 または 姓"></div>
  </div>
  <div class="sec-t">預け荷物 <small>Checked Baggage</small></div>
  <div class="sel-grid g3c" style="margin-bottom:32px">${[{v:0,l:'0個',s:'なし'},{v:1,l:'1個',s:''},{v:2,l:'2個以上',s:''}].map(o=>`<div class="sel-btn ob${o.v===oacS.bags?' act':''}" onclick="oacS.bags=${o.v};selGroup('ob',this)">${o.l}${o.s?`<small>${o.s}</small>`:''}</div>`).join('')}</div>
  <button class="btn bp" style="padding:16px;font-size:16px" onclick="checkOac()">利用可否を確認する</button>
  <div id="oacRes" style="margin-top:24px"></div></section>`;
}
function checkOac(){
  const al=$('oacAl').value,fn=$('oacFn').value.trim(),ap=$('oacAp').value,dt=$('oacDt').value,tm=$('oacTm').value,ref=$('oacRef').value.trim();
  if(!al||!fn||!ap||!dt||!tm||!ref){helpers.toast('すべての項目を入力してください');return}
  Object.assign(oacS,{airline:al,flight:fn,airport:ap,date:dt,time:tm,ref:ref});
  const dep=new Date(dt+'T'+tm+':00'); const diff=(dep-new Date())/(36e5);
  if(diff<3||al==='その他'){oacS.elig='unavailable';oacS.saved=0}
  else if(oacS.bags>=2){oacS.elig='conditional';oacS.saved=60}
  else{oacS.elig='available';oacS.saved=90}
  helpers.toast('確認中...'); setTimeout(showOacResult,600);
}
function showOacResult(){
  const r=$('oacRes'); const dh=parseInt(oacS.time); const dl=Math.max(dh-4,8)+':00';
  if(oacS.elig==='available'){
    r.innerHTML=`<div class="oac-res avl"><div class="oac-rb" style="background:var(--grn)">✓ 利用可能</div><h4 class="fw7 mb2" style="font-size:16px">OACをご利用いただけます</h4><div class="fxc g2 ts fsub"><div class="fx jcsb"><span>締切時刻</span><strong class="fw7" style="color:var(--tx)">${dl} まで</strong></div><div class="fx jcsb"><span>短縮時間</span><strong class="fw7" style="color:var(--grn)">約${oacS.saved}分</strong></div></div></div><button class="btn bp" style="padding:16px;font-size:16px" onclick="goOacConfirm()">チェックインへ進む</button>`;
  }else if(oacS.elig==='conditional'){
    r.innerHTML=`<div class="oac-res cnd"><div class="oac-rb" style="background:var(--org)">⚠ 条件付き利用可</div><h4 class="fw7 mb2" style="font-size:16px">条件付きでOACを利用できます</h4><p class="ts fw7 mb3" style="color:var(--org)">預け荷物が2個以上のため追加時間がかかる場合があります。</p><div class="fxc g2 ts fsub"><div class="fx jcsb"><span>締切時刻</span><strong class="fw7" style="color:var(--tx)">${dl} まで</strong></div><div class="fx jcsb"><span>短縮時間</span><strong class="fw7" style="color:var(--org)">約${oacS.saved}分</strong></div></div></div><button class="btn bp" style="padding:16px;font-size:16px" onclick="goOacConfirm()">条件を確認して進む</button>`;
  }else{
    r.innerHTML=`<div class="oac-res una"><div class="oac-rb" style="background:var(--red)">✕ 利用不可</div><h4 class="fw7 mb2" style="font-size:16px">今回はOACをご利用いただけません</h4><p class="ts fw7" style="color:var(--red)">${oacS.airline==='その他'?'この航空会社はOAC非対応です。':'出発時刻が近いため対象外です。'}</p></div>
    <div class="card" style="background:#F2F2F7;box-shadow:none"><h4 class="ts fw7 mb3">代替案</h4><p class="ts fsub mb3" style="line-height:1.5">空港チェックインをご利用ください。</p><button class="btn ts" style="padding:14px;background:#fff;border:1px solid #E5E5EA" onclick="nav('home')">🏠 ホームへ戻る</button></div>`;
  }
}
const counters=[{k:'tokyo',n:'東京駅 八重洲カウンター',s:'JR東京駅 八重洲中央口 徒歩2分'},{k:'shinjuku',n:'新宿バスタ シティターミナル',s:'新宿駅 南口 直結'},{k:'shinagawa',n:'品川駅 港南口カウンター',s:'JR品川駅 港南口 徒歩1分'}];
const slots=['10:00-10:30','10:30-11:00','11:00-11:30','11:30-12:00','12:00-12:30','12:30-13:00'];
function goOacConfirm(){
  const apN={'NRT':'成田国際空港 (NRT)','HND':'羽田空港 (HND)','KIX':'関西国際空港 (KIX)'};
  const dh=parseInt(oacS.time),dm=parseInt(oacS.time.split(':')[1])||0;
  const rm=dh*60+dm-oacS.saved; const rH=String(Math.floor(rm/60)).padStart(2,'0')+':'+String(rm%60).padStart(2,'0');
  const freeH=Math.floor(oacS.saved/60),freeM=oacS.saved%60;let freeStr='';if(freeH)freeStr+=freeH+'時間';if(freeM)freeStr+=freeM+'分';
  $('v-oac-confirm').innerHTML=helpers.sh('oac-form','チェックイン確認')+`<section class="sec">
  <div class="card"><p class="ts fw7 fsub mb2">フライト情報</p>${[['航空会社・便名',oacS.airline+' '+oacS.flight],['出発空港',apN[oacS.airport]||oacS.airport],['出発日時',oacS.date+' '+oacS.time],['預け荷物',oacS.bags===0?'なし':oacS.bags+'個']].map(r=>`<div class="fx jcsb aic mb2"><span class="ts fsub">${r[0]}</span><span class="fw7 ts">${helpers.esc(r[1])}</span></div>`).join('')}</div>
  <div class="sec-t">チェックイン拠点 <small>Counter</small></div>
  <div style="margin-bottom:16px">${counters.map((c,i)=>`<div class="oac-co${i===0?' act':''}" onclick="oacS.counter='${c.k}';oacS.counterName='${c.n}';$$('.oac-co').forEach(e=>e.classList.remove('act'));this.classList.add('act')"><div class="fx jcsb aic"><div class="fx aic g3"><div class="gi-icon" style="border-radius:50%">${I.flag}</div><div><div class="fw7 ts">${c.n}</div><div class="txs fsub">${c.s}</div></div></div><div class="radio"></div></div></div>`).join('')}</div>
  <div class="sec-t">利用時間帯 <small>Time Slot</small></div>
  <div class="oac-sg">${slots.map((s,i)=>`<div class="oac-sb${i===0?' act':''}" onclick="oacS.slot='${s}';$$('.oac-sb').forEach(e=>e.classList.remove('act'));this.classList.add('act')">${s}</div>`).join('')}</div>
  <div class="oac-ts mt4"><div class="oac-ts-i">${I.clock}</div><div><h4>あと${freeStr}、駅周辺を楽しめます</h4><p>空港到着推奨: <strong>${rH}</strong></p></div></div>
  <button class="btn bp mt4" style="padding:16px;font-size:16px" onclick="confirmOac('${rH}')">OACを確定する</button></section>`;
  nav('oac-confirm');
}
function confirmOac(rH){
  helpers.toast('処理中...'); oacS.refNum='OAC-'+String(10000+Math.floor(Math.random()*89999));
  const passName=(state.profile&&state.profile.name)?state.profile.name.toUpperCase():'GUEST USER';
  setTimeout(()=>{
    const seats=['12A','15C','24A','31F','8B','19D']; const gates=['22','32','45','18','51'];
    const seat=seats[Math.floor(Math.random()*seats.length)], gate=gates[Math.floor(Math.random()*gates.length)];
    addRecord('oac',{refNum:oacS.refNum,airline:oacS.airline,flight:oacS.flight,airport:oacS.airport,date:oacS.date,time:oacS.time,bags:oacS.bags,counter:oacS.counterName,slot:oacS.slot,seat:seat,gate:gate,recommendedArrival:rH});
    $('v-oac-complete').innerHTML=`<div class="sh"><div style="width:32px"></div><h2>チェックイン準備完了</h2></div><section class="sec fxc aic" style="padding-top:24px">
    <div class="succ">${I.check}</div><h2 style="font-size:22px;font-weight:800;margin-bottom:8px">OACの準備が完了しました</h2>
    <div class="card w100 tac"><p class="txs fsub mb2">チェックイン参照番号</p><p style="font-size:24px;font-weight:800;letter-spacing:2px;color:var(--pri-dk)">${oacS.refNum}</p></div>
    <div class="bp-mock w100"><div class="fx jcsb" style="margin-bottom:16px"><div><div class="txs fsub mb2">PASSENGER</div><div class="fw7" style="font-size:16px">${helpers.esc(passName)}</div></div><div class="tar"><div class="txs fsub mb2">FLIGHT</div><div class="fw7" style="font-size:16px">${helpers.esc(oacS.airline.split(' ')[0])} ${helpers.esc(oacS.flight)}</div></div></div>
    <div class="bp-route"><div class="bp-ap"><div class="code">${helpers.esc(oacS.airport)}</div><div class="nm">出発</div></div><div class="bp-arrow">${I.arrow}</div><div class="bp-ap"><div class="code">—</div><div class="nm">到着</div></div></div>
    <div class="fx jcsb" style="margin-bottom:16px">${[['DATE',oacS.date],['TIME',oacS.time],['SEAT',seat],['GATE',gate]].map(r=>`<div><div class="txs fsub">${r[0]}</div><div class="fw7 ts">${r[1]}</div></div>`).join('')}</div></div>
    <div class="card w100"><h4 class="ts fw7 mb3">空港到着推奨</h4><p class="ts fsub">推奨時刻: <strong>${helpers.esc(rH)}</strong></p></div>
    <button class="btn bp mb3" style="padding:16px;font-size:16px" onclick="nav('home')">ホームへ戻る</button>
    <button class="btn bo" style="padding:14px;font-size:14px" onclick="nav('mobility');renderMobility()">空港までの経路を開く</button></section>`;
    nav('oac-complete');
  },800);
}


/* ===== History / Saved Records Views ===== */
function renderHistoryHub(){
  const records=loadRecords();
  const counts={tours:records.tours.length,baggage:records.baggage.length,tickets:records.tickets.length,refunds:records.refunds.length,oac:records.oac.length};
  const total=Object.values(counts).reduce((a,b)=>a+b,0);
  const cats=[
    {id:'history-tours',icon:'tour',label:'観光ガイド',count:counts.tours,emoji:'🗺️'},
    {id:'history-baggage',icon:'bag',label:'手荷物配送',count:counts.baggage,emoji:'🧳'},
    {id:'history-tickets',icon:'ticket',label:'チケット購入',count:counts.tickets,emoji:'🎟️'},
    {id:'history-refunds',icon:'yen',label:'免税リファンド',count:counts.refunds,emoji:'🧾'},
    {id:'history-oac',icon:'plane',label:'OAC',count:counts.oac,emoji:'🛂'}
  ];
  $('v-history-hub').innerHTML=helpers.sh('home','利用履歴')+`<section class="sec">
    <div class="card" style="background:#F0F8FF;border:1px solid #BDE0FE;box-shadow:none;text-align:center;padding:20px">
      <div style="font-size:36px;font-weight:800;color:var(--pri-dk)">${total}</div>
      <div class="ts fsub">件の保存済み記録</div>
    </div>
    ${cats.map(c=>`<div class="hist-card" onclick="nav('${c.id}')">
      <div class="hc-hd"><span class="em">${c.emoji}</span><span class="t">${c.label}</span><span class="badge b-blu">${c.count}件</span></div>
    </div>`).join('')}
  </section>`;
}

function renderHistoryTours(){
  const records=loadRecords();
  const tours=records.tours||[];
  $('v-history-tours').innerHTML=helpers.sh('history-hub','保存した旅行プラン')+`<section class="sec">
    ${tours.length?tours.map((t,i)=>{
      const planNames=(t.plans||[]).slice(0,2).map(p=>p.title||'プラン').join(', ');
      const themes=(t.conditions?.themes||[]).join(', ')||'指定なし';
      return `<div class="hist-card" onclick="openHistoryTourDetail('${t.id}')">
        <div class="hc-hd"><span class="em">🗺️</span><span class="t">${helpers.esc(planNames)}</span><span class="dt">${fmtSavedDate(t.savedAt)}</span></div>
        <div class="hc-body">${helpers.esc(t.location||'')} ・ テーマ: ${helpers.esc(themes)}</div>
        <div class="hc-tags"><span class="badge b-blu">${(t.plans||[]).length}プラン</span></div>
      </div>`;
    }).join(''):`<div class="hist-empty"><div class="em">🗺️</div><div class="t">保存された旅行プランはありません</div><div class="s">観光ガイドでAIプランを作成すると、ここに保存されます。</div></div>`}
    <button class="btn bo mt4" onclick="renderTour();nav('tour')">新しくプランを作成する</button>
  </section>`;
}

function openHistoryTourDetail(id){
  const records=loadRecords();
  const tour=(records.tours||[]).find(t=>t.id===id);
  if(!tour){helpers.toast('データが見つかりません');return;}
  let html=helpers.sh('history-tours','保存済みプラン詳細')+`<section class="sec">
    <div class="card" style="background:#F0F8FF;border:1px solid #BDE0FE;box-shadow:none">
      <div class="fx jcsb aic mb2"><span class="ts fw7" style="color:var(--pri-dk)">📅 保存日時</span><span class="ts fw7">${fmtSavedDate(tour.savedAt)}</span></div>
      <div class="fx jcsb aic mb2"><span class="ts fw7" style="color:var(--pri-dk)">📍 場所</span><span class="ts fw7">${helpers.esc(tour.location||'-')}</span></div>
      <div class="fx jcsb aic mb2"><span class="ts fw7" style="color:var(--pri-dk)">🎯 テーマ</span><span class="ts fw7">${helpers.esc((tour.conditions?.themes||[]).join(', ')||'-')}</span></div>
      <div class="fx jcsb aic mb2"><span class="ts fw7" style="color:var(--pri-dk)">⚡ 体力</span><span class="ts fw7">${helpers.esc(tour.conditions?.energy==='tired'?'少し疲れた':'元気')}</span></div>
      <div class="fx jcsb aic mb2"><span class="ts fw7" style="color:var(--pri-dk)">👥 混雑</span><span class="ts fw7">${helpers.esc(tour.conditions?.crowd==='avoid'?'避けたい':'OK')}</span></div>
      <div class="fx jcsb aic"><span class="ts fw7" style="color:var(--pri-dk)">⏱ 時間</span><span class="ts fw7">${helpers.esc({short:'1〜2時間',half:'半日',full:'1日'}[tour.conditions?.time]||tour.conditions?.time||'-')}</span></div>
      ${tour.conditions?.freeText?`<div class="mt3" style="border-top:1px solid #BDE0FE;padding-top:8px"><span class="ts fsub">自由記述:</span><div class="ts mt2">${helpers.esc(tour.conditions.freeText)}</div></div>`:''}
    </div>`;
  if(tour.intro){
    html+=`<div class="card" style="background:var(--card)"><p class="ts fw7 mb2 fx aic g2">${I.star} AIコメント</p><p class="ts" style="color:var(--pri-dk)">${helpers.esc(tour.intro)}</p></div>`;
  }
  (tour.plans||[]).forEach((plan,i)=>{
    const spots=Array.isArray(plan.main_spots)?plan.main_spots.join(' → '):'';
    html+=`<div class="card${i===0?' flat" style="border-color:var(--pri);border-width:2px':' flat'}">
      <div class="fx aic g2 mb2"><span style="font-size:18px">${i===0?'⭐':'📍'}</span><span class="fw7" style="font-size:15px">${helpers.esc(plan.title||'プラン'+(i+1))}</span>${i===0?'<span class="badge b-blu" style="font-size:10px">おすすめ</span>':''}</div>
      ${plan.summary?`<p class="ts fsub mb2">${helpers.esc(plan.summary)}</p>`:''}
      ${plan.reason_for_you?`<div style="background:#F0F8FF;border:1px solid #BDE0FE;border-radius:8px;padding:8px 12px;margin-bottom:8px"><p class="ts" style="color:var(--pri-dk);line-height:1.5">💡 ${helpers.esc(plan.reason_for_you)}</p></div>`:''}
      <div class="fx g2 mb2" style="flex-wrap:wrap">
        ${plan.crowd_level?`<span class="badge ${crowdBadgeClass(plan.crowd_level)}">混雑: ${helpers.esc(plan.crowd_level)}</span>`:''}
        ${plan.rest_level?`<span class="badge ${restBadgeClass(plan.rest_level)}">休憩: ${helpers.esc(plan.rest_level)}</span>`:''}
        ${plan.duration?`<span class="badge b-blu">所要: ${helpers.esc(plan.duration)}</span>`:''}
      </div>
      ${spots?`<p class="ts mb2">🗺️ ${helpers.esc(spots)}</p>`:''}
      ${Array.isArray(plan.rest_spots)&&plan.rest_spots.length?`<p class="ts fsub">☕ ${helpers.esc(plan.rest_spots.join(', '))}</p>`:''}
    </div>`;
  });
  html+=`<button class="hist-del-btn" onclick="deleteRecord('tours','${tour.id}');helpers.toast('削除しました');nav('history-tours')">🗑 この記録を削除</button>`;
  html+=`</section>`;
  $('v-history-tour-detail').innerHTML=html;
  nav('history-tour-detail');
}

function renderHistoryBaggage(){
  const records=loadRecords();
  const list=records.baggage||[];
  $('v-history-baggage').innerHTML=helpers.sh('history-hub','手荷物配送 予約履歴')+`<section class="sec">
    ${list.length?list.map(b=>`<div class="hist-card" onclick="openHistoryBaggageDetail('${b.id}')">
      <div class="hc-hd"><span class="em">🧳</span><span class="t">${helpers.esc(b.refNum||'-')}</span><span class="dt">${fmtSavedDate(b.savedAt)}</span></div>
      <div class="hc-body">${helpers.esc(b.drop||'')} → ${helpers.esc(b.dest||'')}${b.hotel?' ('+helpers.esc(b.hotel)+')':''}</div>
      <div class="hc-tags"><span class="badge b-grn">${helpers.esc(b.status||'予約済み')}</span><span class="badge b-blu">${helpers.esc(b.size||'')} x ${helpers.esc(b.qtyLabel||b.qty)}</span></div>
    </div>`).join(''):`<div class="hist-empty"><div class="em">🧳</div><div class="t">予約履歴はありません</div><div class="s">手荷物配送を予約すると、ここに記録されます。</div></div>`}
    <button class="btn bo mt4" onclick="renderBagForm();nav('bag-form')">新しく予約する</button>
  </section>`;
}

function openHistoryBaggageDetail(id){
  const records=loadRecords();
  const b=(records.baggage||[]).find(r=>r.id===id);
  if(!b){helpers.toast('データが見つかりません');return;}
  $('v-history-baggage-detail').innerHTML=helpers.sh('history-baggage','予約詳細')+`<section class="sec">
    <div class="card tac"><p class="txs fsub mb2">予約番号</p><p style="font-size:24px;font-weight:800;letter-spacing:1px;color:var(--pri-dk)">${helpers.esc(b.refNum||'-')}</p></div>
    <div class="card">
      <div class="wd-row"><span>予約日時</span><span>${fmtSavedDate(b.savedAt)}</span></div>
      <div class="wd-row"><span>状態</span><span><span class="badge b-grn">${helpers.esc(b.status||'予約済み')}</span></span></div>
      <div class="wd-row"><span>荷物</span><span>${helpers.esc(b.size||'')} x ${helpers.esc(b.qtyLabel||b.qty)}</span></div>
      <div class="wd-row"><span>預け場所</span><span>${helpers.esc(b.drop||'-')}</span></div>
      <div class="wd-row"><span>届け先</span><span>${helpers.esc(b.dest||'-')}</span></div>
      ${b.hotel?`<div class="wd-row"><span>ホテル名</span><span>${helpers.esc(b.hotel)}</span></div>`:''}
    </div>
    <button class="hist-del-btn" onclick="deleteRecord('baggage','${b.id}');helpers.toast('削除しました');nav('history-baggage')">🗑 この記録を削除</button>
  </section>`;
  nav('history-baggage-detail');
}

function renderHistoryTickets(){
  const records=loadRecords();
  const list=records.tickets||[];
  $('v-history-tickets').innerHTML=helpers.sh('history-hub','チケット購入履歴')+`<section class="sec">
    ${list.length?list.map(t=>`<div class="hist-card">
      <div class="hc-hd"><span class="em">${t.ticketEmoji||'🎟️'}</span><span class="t">${helpers.esc(t.ticketName||'-')}</span><span class="dt">${fmtSavedDate(t.savedAt)}</span></div>
      <div class="hc-body">${helpers.esc(t.refNum||'')} ・ ${helpers.esc(t.date||'')} ・ 大人${t.adult} 子${t.child}</div>
      <div class="hc-tags"><span class="badge b-blu">¥ ${(t.total||0).toLocaleString()}</span></div>
    </div>`).join(''):`<div class="hist-empty"><div class="em">🎟️</div><div class="t">購入履歴はありません</div><div class="s">チケットを購入すると、ここに記録されます。</div></div>`}
  </section>`;
}

function renderHistoryRefunds(){
  const records=loadRecords();
  const list=records.refunds||[];
  $('v-history-refunds').innerHTML=helpers.sh('history-hub','免税リファンド履歴')+`<section class="sec">
    ${list.length?list.map(r=>`<div class="hist-card">
      <div class="hc-hd"><span class="em">🧾</span><span class="t">免税申請</span><span class="dt">${fmtSavedDate(r.savedAt)}</span></div>
      <div class="hc-body">${r.itemCount||0}件 ・ 購入総額 ¥${(r.total||0).toLocaleString()}</div>
      <div class="hc-tags"><span class="badge b-grn">還付 約¥${(r.refundAmt||0).toLocaleString()}</span></div>
    </div>`).join(''):`<div class="hist-empty"><div class="em">🧾</div><div class="t">免税履歴はありません</div><div class="s">免税申請を行うと、ここに記録されます。</div></div>`}
  </section>`;
}

function renderHistoryOac(){
  const records=loadRecords();
  const list=records.oac||[];
  $('v-history-oac').innerHTML=helpers.sh('history-hub','OAC履歴')+`<section class="sec">
    ${list.length?list.map(o=>`<div class="hist-card">
      <div class="hc-hd"><span class="em">🛂</span><span class="t">${helpers.esc(o.refNum||'-')}</span><span class="dt">${fmtSavedDate(o.savedAt)}</span></div>
      <div class="hc-body">${helpers.esc(o.airline||'')} ${helpers.esc(o.flight||'')} ・ ${helpers.esc(o.date||'')} ${helpers.esc(o.time||'')}</div>
      <div class="hc-tags"><span class="badge b-blu">${helpers.esc(o.airport||'')}</span><span class="badge b-grn">Seat ${helpers.esc(o.seat||'-')}</span></div>
    </div>`).join(''):`<div class="hist-empty"><div class="em">🛂</div><div class="t">OAC履歴はありません</div><div class="s">OACチェックインを行うと、ここに記録されます。</div></div>`}
  </section>`;
}

/* ── AI Chat: multi-provider support ── */
const chatHistory=[];

/* ===== Action Registry (Whitelist) ===== */
/* TODO: 本番公開時はAPIキーをブラウザに置かず、サーバー側proxy endpoint経由でAI APIを呼び出すこと。 */
const ACTION_REGISTRY = {
  open_view(params)      { if(params.view) nav(params.view); },
  set_mobility(params)   { if(params.destination) state.mobility.destination=params.destination; if(params.origin) state.mobility.origin=params.origin; if(params.mode){ state.mobility.mode=params.mode; tourS&&(tourS.energy=tourS.energy); } saveState(); renderMobility(); nav('mobility'); },
  suggest_ticket(params) { openTicketFromMode(params.mode||null); },
  open_baggage_draft(p)  { renderBagForm(); nav('bag-form'); },
  open_oac_check()       { renderOacForm(); nav('oac-form'); },
  open_refund_check()    { renderRefundForm(); nav('refund-form'); },
  open_tour_plan()       { renderTour(); nav('tour'); },
  open_emergency_help()  { renderTrouble(); nav('trouble'); }
};

function executeAIAction(action){
  if(!action||!action.type) return;
  const fn = ACTION_REGISTRY[action.type];
  if(fn){
    try{ fn(action); }catch(e){ console.error('Action exec error:',e); }
  }else{
    console.warn('Unknown action type:', action.type);
  }
}

/* ===== Local Next-Action Generator ===== */
function generateLocalNextActions(){
  const actions = [];
  const w = state.weather?.current;
  const todos = visibleTodos();
  const M = state.mobility;

  /* Priority 1: Emergency / safety – currently no runtime signal, skip */

  /* Priority 2: Pre-departure procedures */
  const oacTodo = todos.find(t=>t.id==='oac');
  if(oacTodo) actions.push({icon:'🛂',title:'OACの確認をしましょう',summary:'空港外チェックインの利用可否を確認できます。',badge:'帰国準備',cls:'warn',action:{type:'open_oac_check',label:'OACを確認する'}});
  const refundTodo = todos.find(t=>t.id==='refund');
  if(refundTodo) actions.push({icon:'🧾',title:'免税手続きを確認しましょう',summary:'購入した免税品とレシートの整理をしましょう。',badge:'帰国準備',cls:'warn',action:{type:'open_refund_check',label:'免税を確認する'}});

  /* Priority 3: Weather */
  if(w){
    const rainy=[51,53,55,61,63,65,80,81,82,95,96,99];
    if(rainy.includes(w.code)) actions.push({icon:'☂️',title:'雨の予報です',summary:'傘を持って、屋内中心の観光がおすすめです。',badge:'天気',cls:'',action:{type:'open_tour_plan',label:'屋内プランを提案'}});
  }

  /* Priority 4: IC balance */
  if(state.balance<1000) actions.push({icon:'💳',title:'IC残高が少なくなっています',summary:`残高 ¥${state.balance.toLocaleString()}。移動前にチャージしましょう。`,badge:'交通',cls:'warn',action:{type:'open_view',label:'チャージする',view:'charge'}});

  /* Priority 5: Resume route */
  if(M.destination) actions.push({icon:'🚃',title:`${M.destination} への経路`,summary:'前回検索した目的地への経路を確認できます。',badge:'移動',cls:'',action:{type:'set_mobility',label:'経路を開く',destination:M.destination,origin:M.origin||'',mode:M.mode}});

  /* Priority 6: Nearby spots */
  if(state.nearbySpots.length>0 && actions.length<3){
    const top=state.nearbySpots[0];
    actions.push({icon:top.emoji||'📍',title:`${top.name} が近くにあります`,summary:`${helpers.formatDistance(top.distanceKm)} – ${(top.desc||'').slice(0,30)}`,badge:'おすすめ',cls:'',action:{type:'open_tour_plan',label:'観光プランを見る'}});
  }

  /* Priority 7: Remaining todos */
  const docsTodo = todos.find(t=>t.id==='docs');
  if(docsTodo && actions.length<3) actions.push({icon:'📄',title:'出発前の書類確認',summary:'パスポート・ビザ・保険を再確認しましょう。',badge:'確認',cls:'',action:{type:'open_view',label:'確認する',view:'todo-detail'}});

  return actions.slice(0,3);
}

/* ===== AI Carousel State ===== */
let _aiCarouselIdx = 0;
let _aiCarouselTimer = null;
let _aiCarouselCount = 0;
let _aiCarouselTouchStartX = 0;
let _aiCarouselTouchDelta = 0;

function slideAICarousel(idx, resetTimer){
  if(_aiCarouselCount<=0) return;
  _aiCarouselIdx = ((idx % _aiCarouselCount) + _aiCarouselCount) % _aiCarouselCount;
  const track = document.querySelector('.ai-carousel-track');
  if(track) track.style.transform = `translateX(-${_aiCarouselIdx * 100}%)`;
  document.querySelectorAll('.ai-dot').forEach((d,i)=>d.classList.toggle('act', i===_aiCarouselIdx));
  if(resetTimer) resetAICarouselTimer();
}

function resetAICarouselTimer(){
  if(_aiCarouselTimer) clearInterval(_aiCarouselTimer);
  if(_aiCarouselCount>1){
    _aiCarouselTimer = setInterval(()=>slideAICarousel(_aiCarouselIdx+1, false), 10000);
  }
}

function stopAICarouselTimer(){
  if(_aiCarouselTimer){ clearInterval(_aiCarouselTimer); _aiCarouselTimer=null; }
}

/* ===== Render Home AI Section (Carousel) ===== */
let _homeAIActions = []; /* Store action objects for safe button dispatch */
function renderHomeAI(){
  const el=$('homeAI'); if(!el) return;
  stopAICarouselTimer();
  const av=getSelectedAvatar();
  const cards = generateLocalNextActions();
  _homeAIActions = cards.map(c=>c.action);
  _aiCarouselCount = cards.length;
  _aiCarouselIdx = 0;
  if(!cards.length){ el.innerHTML=''; return; }

  /* Build dots */
  const dots = cards.map((_,i)=>`<button class="ai-dot${i===0?' act':''}" onclick="slideAICarousel(${i},true)"></button>`).join('');

  let html=`<div class="ai-next">
    <div class="ai-next-hd">
      <img src="${av.imgSm}" style="width:28px;height:28px;border-radius:50%;object-fit:cover;border:2px solid ${av.theme.pri};flex-shrink:0">
      <span class="ai-label">${helpers.esc(av.name)}からの次アクション</span>
      ${cards.length>1?`<div class="ai-dots">${dots}</div>`:''}
    </div>
    <div class="ai-carousel" id="aiCarousel">
      <div class="ai-carousel-track">`;

  cards.forEach((c,idx)=>{
    html+=`<div class="ai-carousel-slide">
      <div class="ai-card ${c.cls||''}">
        <div class="ai-card-row">
          <div class="ai-card-icon">${c.icon}</div>
          <div class="ai-card-body">
            <div class="ai-card-title">${helpers.esc(c.title)} ${c.badge?`<span class="ai-card-badge">${helpers.esc(c.badge)}</span>`:''}</div>
            <div class="ai-card-summary">${helpers.esc(c.summary)}</div>
            <button class="ai-action-btn" onclick="executeHomeAIAction(${idx})">${helpers.esc(c.action.label||'確認する')}</button>
          </div>
        </div>
      </div>
    </div>`;
  });

  html+=`</div></div></div>`;
  el.innerHTML=html;

  /* Setup swipe */
  if(cards.length>1){
    const carousel = $('aiCarousel');
    if(carousel){
      carousel.addEventListener('touchstart', e=>{
        _aiCarouselTouchStartX = e.touches[0].clientX;
        _aiCarouselTouchDelta = 0;
      }, {passive:true});
      carousel.addEventListener('touchmove', e=>{
        _aiCarouselTouchDelta = e.touches[0].clientX - _aiCarouselTouchStartX;
      }, {passive:true});
      carousel.addEventListener('touchend', ()=>{
        if(Math.abs(_aiCarouselTouchDelta)>40){
          if(_aiCarouselTouchDelta<0) slideAICarousel(_aiCarouselIdx+1, true);
          else slideAICarousel(_aiCarouselIdx-1, true);
        }
        _aiCarouselTouchDelta = 0;
      }, {passive:true});
    }
    resetAICarouselTimer();
  }
}
function executeHomeAIAction(idx){
  const action = _homeAIActions[idx];
  if(action) executeAIAction(action);
}

/* ===== Build App Context for AI ===== */
function buildAppContext(){
  const p=state.profile||{}, L=state.location;
  const loc=(L.permission==='granted'&&L.label)?L.label:(L.fallback||'東京');
  const w=state.weather?.current;
  const spots=state.nearbySpots.slice(0,5).map(s=>s.name+' ('+helpers.formatDistance(s.distanceKm)+')');
  const todos=visibleTodos().map(t=>t.title);

  return `## appContext
profile:
  name: ${p.name||'ゲスト'}
  nationality: ${p.nationality||'不明'}
  languages: ${(p.languages||[]).join(', ')||'日本語'}
  age: ${p.age||'不明'}
  preferences: ${(p.preferences||[]).join(', ')||'不明'}
  japanVisitCount: ${p.japanVisitCount||'不明'}
location: ${loc}
${w?`weather: ${helpers.mapWeatherToIcon(w.code).label} ${w.temp}℃ (${helpers.getClothingAdvice(w.temp,w.code)})`:'weather: 不明'}
nearbySpots: ${spots.length?spots.join(', '):'なし'}
todos: ${todos.length?todos.join(', '):'なし'}
mobility: origin=${state.mobility.origin||'未設定'}, destination=${state.mobility.destination||'未設定'}, mode=${state.mobility.mode}
balance: ¥${state.balance.toLocaleString()}
currentView: ${state.currentView}
capabilities:
  - open_view { view } — 画面遷移
  - set_mobility { origin, destination, mode } — 経路設定して検索画面へ
  - suggest_ticket { mode } — チケット購入画面へ
  - open_baggage_draft { destination, bags } — 手荷物配送フォームへ
  - open_oac_check — OAC確認フォームへ
  - open_refund_check — 免税確認フォームへ
  - open_tour_plan — 観光ガイドへ
  - open_emergency_help — トラブル・SOSへ
safetyRules:
  - 緊急時は119(救急)または110(警察)を明確に案内
  - チケット購入確定、決済、OAC確定、免税申請、個人情報変更は自動実行しない。必ず確認画面へ案内する。`;
}

/* ===== System Prompt ===== */
const DEFAULT_SYSTEM_PROMPT_TEMPLATE = `あなたは「AssisTrip AI コンシェルジュ」、案内人のつむぎです。
日本を旅行中のユーザーに対して、移動、観光、天気、手荷物、チケット、免税、OAC、SOSを横断して支援します。
あなたの役割は、質問に答えることだけではありません。
ユーザーの状況から「次に何をすべきか」を判断し、アプリ内機能へ安全に導いてください。

回答は原則として次のJSON形式で返してください。
{"message":"2〜4文の短い案内。日本語中心。必要に応じて英語を併記。","cards":[],"actions":[],"requiresConfirmation":false}

cardsの各要素:
{"type":"route|spot|ticket|baggage|weather|todo|oac|refund|emergency","title":"カードタイトル","summary":"短い説明","badge":"任意のバッジ","primaryAction":{"type":"open_view|set_mobility|suggest_ticket|open_baggage_draft|open_oac_check|open_refund_check|open_tour_plan|open_emergency_help","label":"ボタン文言","view":"任意","destination":"任意","origin":"任意","mode":"任意"}}

ルール:
- 可能な場合は、必ずcardsを1つ以上含める。
- 移動相談ではrouteカードを出す。set_mobilityで目的地を設定する。
- 観光相談ではspotまたはtourカードを出す。
- 荷物相談ではbaggageカードを出す。
- 帰国・空港・チェックイン相談ではOACと免税チェックを提案する。
- 体調不良・事故・災害・紛失ではemergencyカードを優先する。
- 命の危険がある場合は119または110を明確に案内する。
- チケット購入確定、決済、OAC確定、免税申請、個人情報変更は自動実行しない。必ず確認画面へ案内する。
- 不確かなことは断定しない。
- 長文ではなく、次に押せるボタンが明確な返答にする。
- JSONとして不正にならないよう注意する。`;

function buildSystemPrompt(){
  const customPrompt = getAdminSetting('aiSystemPrompt','').trim();
  const context = buildAppContext();
  const av = getSelectedAvatar();
  const avatarTone = `\n## ガイドキャラクター\nあなたの名前は「${av.name}」です。\n口調の指針: ${av.tone}\nただし、キャラクターの口調は控えめに反映し、情報の正確さと実用性を最優先してください。`;
  if(customPrompt){
    return customPrompt + avatarTone + '\n' + context;
  }
  return DEFAULT_SYSTEM_PROMPT_TEMPLATE + avatarTone + '\n' + context;
}

async function callAI(userMessage){
  chatHistory.push({role:'user',content:userMessage});
  const trimmed=chatHistory.length>20?chatHistory.slice(-20):chatHistory;
  const provider = getAdminSetting('aiProvider','claude');
  const systemPrompt = buildSystemPrompt();

  try{
    let text = '';

    if(provider === 'openai'){
      const apiKey = getAdminSetting('openAiApiKey','');
      if(!apiKey) throw new Error('OpenAI APIキーが未設定です。管理者設定から設定してください。');
      const msgs = [{role:'system',content:systemPrompt}, ...trimmed];
      const response = await fetchWithRetry('https://api.openai.com/v1/chat/completions',{
        method:'POST',
        headers:{'Content-Type':'application/json','Authorization':'Bearer '+apiKey},
        body:JSON.stringify({model:'gpt-4o-mini',max_tokens:4096,messages:msgs})
      });
      const data = await response.json();
      text = data.choices?.[0]?.message?.content || '';

    }else if(provider === 'gemini'){
      const apiKey = getAdminSetting('geminiApiKey','');
      if(!apiKey) throw new Error('Gemini APIキーが未設定です。管理者設定から設定してください。');
      const contents = trimmed.map(m=>({role:m.role==='assistant'?'model':'user',parts:[{text:m.content}]}));
      const response = await fetchWithRetry(`https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key=${apiKey}`,{
        method:'POST',
        headers:{'Content-Type':'application/json'},
        body:JSON.stringify({
          system_instruction:{parts:[{text:systemPrompt}]},
          contents:contents,
          generationConfig:{
            maxOutputTokens:4096,
            thinkingConfig:{thinkingBudget:0}
          }
        })
      });
      const data = await response.json();
      text = (data.candidates?.[0]?.content?.parts||[]).filter(p=>!p.thought).map(p=>p.text).filter(Boolean).join('\n') || '';

    }else{
      /* Claude (default) */
      const apiKey = getAdminSetting('claudeApiKey','');
      if(!apiKey) throw new Error('Claude APIキーが未設定です。管理者設定から設定してください。');
      const response = await fetchWithRetry('https://api.anthropic.com/v1/messages',{
        method:'POST',
        headers:{'Content-Type':'application/json','x-api-key':apiKey,'anthropic-version':'2023-06-01','anthropic-dangerous-direct-browser-access':'true'},
        body:JSON.stringify({model:'claude-sonnet-4-20250514',max_tokens:4096,system:systemPrompt,messages:trimmed})
      });
      const data = await response.json();
      text = data.content.filter(b=>b.type==='text').map(b=>b.text).join('\n');
    }

    chatHistory.push({role:'assistant',content:text});
    return text;
  }catch(e){
    chatHistory.pop();
    throw e;
  }
}

/* ===== Parse AI JSON Response ===== */
function tryParseAIJSON(raw){
  if(!raw || typeof raw !== 'string') return null;
  /* Strategy 1: Direct parse */
  try{
    const parsed = JSON.parse(raw.trim());
    if(parsed && typeof parsed.message === 'string') return parsed;
  }catch(e){}
  /* Strategy 2: Strip code fences */
  try{
    const fenceMatch = raw.match(/```(?:json)?\s*\n?([\s\S]*?)\n?\s*```/i);
    if(fenceMatch){
      const parsed = JSON.parse(fenceMatch[1].trim());
      if(parsed && typeof parsed.message === 'string') return parsed;
    }
  }catch(e){}
  /* Strategy 3: Extract first JSON object */
  try{
    const firstBrace = raw.indexOf('{');
    const lastBrace = raw.lastIndexOf('}');
    if(firstBrace !== -1 && lastBrace > firstBrace){
      const parsed = JSON.parse(raw.substring(firstBrace, lastBrace + 1));
      if(parsed && typeof parsed.message === 'string') return parsed;
    }
  }catch(e){}
  return null;
}

/* ===== Render AI Response (JSON cards + NAV fallback) ===== */
function renderAIResponse(raw){
  /* 1. Try JSON with cards */
  const json = tryParseAIJSON(raw);
  if(json){
    let html = helpers.esc(json.message||'').replace(/\n/g,'<br>');
    /* Render cards */
    if(json.cards && json.cards.length){
      html += '<div class="chat-card-list">';
      json.cards.forEach((card,ci)=>{
        const actionData = card.primaryAction ? helpers.esc(JSON.stringify(card.primaryAction)) : '';
        html += `<div class="chat-ai-card">
          <div class="cac-title">${helpers.esc(card.title||'')}${card.badge?` <span class="cac-badge">${helpers.esc(card.badge)}</span>`:''}</div>
          ${card.summary?`<div class="cac-summary">${helpers.esc(card.summary)}</div>`:''}
          ${card.primaryAction?`<button class="cac-btn" data-ai-action="${actionData}">${helpers.esc(card.primaryAction.label||'開く')}</button>`:''}
        </div>`;
      });
      html += '</div>';
    }
    /* Render standalone actions as buttons */
    if(json.actions && json.actions.length){
      json.actions.forEach(act=>{
        const actData = helpers.esc(JSON.stringify(act));
        html += `<br><span class="chat-action" data-ai-action="${actData}">👉 ${helpers.esc(act.label||act.type||'実行')}</span>`;
      });
    }
    return html;
  }

  /* 2. Fallback: [NAV:viewId:label] legacy format */
  const navRegex=/\[NAV:([a-z\-]+):(.+?)\]/g;
  const acts=[]; let m;
  while((m=navRegex.exec(raw))!==null) acts.push({v:m[1],l:m[2]});
  let html=helpers.esc(raw.replace(navRegex,'').trim()).replace(/\n/g,'<br>');
  acts.forEach(a=>{ html+=`<br><span class="chat-action" data-nav="${helpers.esc(a.v)}">👉 ${helpers.esc(a.l)}</span>`; });
  return html;
}
let chatSending=false;
function initChatGreeting(){
  const p=state.profile||{};
  const av=getSelectedAvatar();
  const greet=p.name?av.greet.replace(/。$/,'、')+`${p.name}さん。`:av.greet;
  $('chatMsgs').innerHTML=`<div class="msg msg-ai"><div class="fx aic g2 mb2"><img src="${av.imgSm}" style="width:32px;height:32px;border-radius:50%;object-fit:cover;border:2px solid ${av.theme.pri}"><span class="fw7">${helpers.esc(av.name)}</span></div>${helpers.esc(greet)}<br>日本の旅で困ったことはありませんか？移動・観光・手続き、何でもご相談ください。</div>`;
}
function openChat(msg){
  setAvatarMood('normal');
  $('chatOv').classList.add('open');
  if(msg){ $('chatIn').value=msg; $('sendB').disabled=false; setTimeout(doSend,300); }
  else{ $('chatIn').value=''; $('sendB').disabled=true; }
}
function closeChat(){ $('chatOv').classList.remove('open'); }
function qMsg(t){ $('chatIn').value=t; $('sendB').disabled=false; doSend(); }
function addMsg(html,sender){
  const d=document.createElement('div');
  d.className='msg msg-'+(sender==='usr'?'usr':'ai');
  d.innerHTML=html;
  $('chatMsgs').appendChild(d);
  $('chatMsgs').scrollTop=$('chatMsgs').scrollHeight;
  if(sender==='ai'){
    /* Legacy [NAV:...] buttons */
    d.querySelectorAll('.chat-action[data-nav]').forEach(btn=>{
      btn.addEventListener('click',()=>{
        const v=btn.dataset.nav; closeChat();
        const map={
          'mobility-hub':renderMobilityHub,'mobility':renderMobility,
          'ticket':()=>openTicketFromMode(null),
          'baggage':renderBaggage, 'tour':renderTour, 'trouble':renderTrouble,
          'refund':renderRefund, 'oac':renderOac,
          'charge':renderCharge, 'tap':renderTap, 'pay-top':renderPayTop, 'settings':renderSettings
        };
        if(map[v]) map[v]();
        if(v==='ticket') return;
        nav(v);
      });
    });
    /* New JSON action buttons */
    d.querySelectorAll('[data-ai-action]').forEach(btn=>{
      btn.addEventListener('click',()=>{
        try{
          const action=JSON.parse(btn.dataset.aiAction);
          closeChat();
          executeAIAction(action);
        }catch(e){ console.error('AI action parse error:',e); }
      });
    });
  }
  return d;
}
function showTyping(){
  setAvatarMood('thinking');
  const d=document.createElement('div'); d.className='typing'; d.id='typingIndicator';
  d.innerHTML='<span></span><span></span><span></span>';
  $('chatMsgs').appendChild(d); $('chatMsgs').scrollTop=$('chatMsgs').scrollHeight;
}
function hideTyping(){ setAvatarMood('normal'); const e=$('typingIndicator'); if(e) e.remove(); }
async function doSend(){
  const t=$('chatIn').value.trim();
  if(!t||chatSending) return;
  chatSending=true;
  addMsg(helpers.esc(t),'usr');
  $('chatIn').value=''; $('sendB').disabled=true;
  showTyping();
  try{ const res=await callAI(t); hideTyping(); addMsg(renderAIResponse(res),'ai'); }
  catch(e){ hideTyping(); addMsg('エラー: '+helpers.esc(e.message||'通信に失敗しました。しばらくしてから再度お試しください。'),'ai'); }
  finally{ chatSending=false; }
}


/* ===== RPG Welcome Screen ===== */
let _rpgStep=0, _rpgTyping=false, _rpgTimer=null, _rpgLines=[];
function showRpgWelcome(){
  const av=getSelectedAvatar();
  const userName=(state.profile&&state.profile.name)?state.profile.name:'旅人';
  _rpgLines=[
    {name:av.name, text:`${av.theme.greetEmoji} ようこそ、${userName}さん。\n日本への旅が、今始まります。`},
    {name:av.name, text:`私の名前は「${av.name}」。\nあなた専用の旅のコンシェルジュです。`},
    {name:av.name, text:`移動、観光、手荷物、チケット、\nトラブル対応…何でもお任せください。`},
    {name:av.name, text:`さあ、一緒に素敵な旅を\n始めましょう！ ✨`}
  ];
  _rpgStep=0;
  /* Generate stars */
  const starsEl=$('rpgStars');
  let starHtml='';
  for(let i=0;i<60;i++){
    const x=Math.random()*100, y=Math.random()*70, d=Math.random()*3, s=1+Math.random()*2;
    starHtml+=`<div class="rpg-star" style="left:${x}%;top:${y}%;animation-delay:${d}s;width:${s}px;height:${s}px"></div>`;
  }
  starsEl.innerHTML=starHtml;
  /* Set character - use rpgImg if available (transparent bg), else img */
  const rpgSrc=av.rpgImg||av.img;
  $('rpgCharaImg').src=rpgSrc;
  /* Detect JPEG vs SVG for styling */
  const isJpg=rpgSrc.startsWith('data:image/jpeg');
  $('rpgChara').classList.toggle('is-jpg',isJpg);
  /* Show overlay */
  $('rpgOverlay').classList.add('active');
  setTimeout(()=>typeRpgLine(),900);
}
function typeRpgLine(){
  if(_rpgStep>=_rpgLines.length){ closeRpgWelcome(); return; }
  const line=_rpgLines[_rpgStep];
  $('rpgName').textContent=line.name;
  $('rpgTap').style.visibility='hidden';
  const textEl=$('rpgText');
  textEl.innerHTML='';
  _rpgTyping=true;
  let charIdx=0;
  const chars=line.text;
  if(_rpgTimer) clearInterval(_rpgTimer);
  _rpgTimer=setInterval(()=>{
    if(charIdx>=chars.length){
      clearInterval(_rpgTimer); _rpgTimer=null; _rpgTyping=false;
      textEl.innerHTML=chars.replace(/\n/g,'<br>')+'<span class="rpg-cursor"></span>';
      $('rpgTap').style.visibility='visible';
      return;
    }
    charIdx++;
    textEl.innerHTML=chars.substring(0,charIdx).replace(/\n/g,'<br>')+'<span class="rpg-cursor"></span>';
  },45);
}
function advanceRpgDialog(){
  if(_rpgTyping){
    /* Skip typing, show full text */
    if(_rpgTimer){clearInterval(_rpgTimer);_rpgTimer=null;}
    _rpgTyping=false;
    const line=_rpgLines[_rpgStep];
    $('rpgText').innerHTML=line.text.replace(/\n/g,'<br>')+'<span class="rpg-cursor"></span>';
    $('rpgTap').style.visibility='visible';
    return;
  }
  _rpgStep++;
  if(_rpgStep>=_rpgLines.length){ closeRpgWelcome(); }
  else{ typeRpgLine(); }
}
function closeRpgWelcome(){
  if(_rpgTimer){clearInterval(_rpgTimer);_rpgTimer=null;}
  const ov=$('rpgOverlay');
  ov.style.transition='opacity .6s';
  ov.style.opacity='0';
  setTimeout(()=>{ov.classList.remove('active');ov.style.opacity='';ov.style.transition='';},600);
}

(function init(){
  loadState();
  applyAvatarTheme();
  updateAvatarUI();
  $('hamBtn').onclick=openMenu;
  $('menuOv').onclick=closeMenu;
  $('chatFab').onclick=()=>openChat();
  $('chatClose').onclick=closeChat;
  $('chatOv').onclick=closeChat;
  $('chatIn').oninput=e=>{$('sendB').disabled=!e.target.value.trim()};
  $('chatIn').onkeypress=e=>{if(e.key==='Enter'&&$('chatIn').value.trim())doSend()};
  $('sendB').onclick=doSend;
  renderLogin();
  renderPayTop(); renderCharge(); renderTap(); renderIcManage();
  renderMobilityHub(); renderMobility(); renderBaggage(); renderTour(); renderTrouble(); renderRefund(); renderOac();
  updBal(); initChatGreeting();
  if(!state.session.isLoggedIn){ nav('login'); }
  else if(!state.profile||!state.profile.name){ renderProfileSetup(); nav('profile-setup'); }
  else{
    renderHome(); renderSettings(); nav('home');
    refreshHomeData();
  }
  updateAdminUI();
})();
</script>
<div class="rpg-overlay" id="rpgOverlay">
  <div class="rpg-bg">
    <div class="rpg-stars" id="rpgStars"></div>
  </div>
  <button class="rpg-skip" onclick="closeRpgWelcome()">スキップ ▸</button>
  <div class="rpg-chara-wrap" id="rpgChara">
    <img id="rpgCharaImg" src="" alt="Guide">
    <div class="rpg-chara-glow"></div>
  </div>
  <div class="rpg-dialog" id="rpgDialog" onclick="advanceRpgDialog()">
    <div class="rpg-name" id="rpgName"></div>
    <div class="rpg-text" id="rpgText"></div>
    <div class="rpg-tap" id="rpgTap">▼ タップして続ける</div>
  </div>
</div>
</body>
</html>
