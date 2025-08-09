<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ashu Gaming - Portfolio</title>
  <meta name="description" content="Ashu Gaming - portfolio. Web developer, bots, and gaming projects." />

  <style>
    :root{
      --bg: #2e2e2e;
      --card: #3c3c3c;
      --muted: #cfcfcf;
      --accent1: #00aaff;
      --accent2: #0066ff;
      --glass: rgba(255,255,255,0.04);
      --radius: 14px;
      --maxw: 920px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter, system-ui, Arial, sans-serif;
      background:linear-gradient(180deg,var(--bg),#242424);
      color:#fff;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:28px;
    }

    .wrap{
      width:100%;
      max-width:var(--maxw);
      display:grid;
      grid-template-columns: 1fr 380px;
      gap:28px;
      align-items:start;
    }

    /* Responsive */
    @media (max-width:880px){
      .wrap{grid-template-columns:1fr; padding:0}
      header .title { font-size:26px }
    }

    /* Left/main column */
    main{
      background:linear-gradient(180deg,var(--card),#333);
      border-radius:var(--radius);
      padding:22px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.5);
    }
    header{display:flex;gap:18px;align-items:center}
    .avatar{
      width:84px;height:84px;border-radius:16px;background:linear-gradient(135deg,var(--accent1),var(--accent2));
      display:flex;align-items:center;justify-content:center;font-weight:700;color:#fff;font-size:28px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.5);
    }
    .title{
      font-size:30px;margin:0;
      letter-spacing:0.6px;
    }
    .subtitle{color:var(--muted);margin-top:6px;font-size:14px}
    p.lead{margin:16px 0;line-height:1.6;color:#e8e8e8}

    .cards{display:flex;gap:12px;flex-wrap:wrap}
    .card{
      background:var(--glass);border-radius:12px;padding:12px 14px;flex:1;min-width:140px;
      border:1px solid rgba(255,255,255,0.03);
    }
    .card h4{margin:0 0 6px 0;font-size:14px}
    .card p{margin:0;color:var(--muted);font-size:13px}

    /* Right / sidebar */
    aside{
      background:linear-gradient(180deg,#343434,#2f2f2f);
      border-radius:var(--radius); padding:18px; min-height:220px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.45);
      position:relative;
    }
    .section-title{font-weight:700;margin-bottom:10px}
    .info p{margin:8px 0;color:var(--muted);font-size:14px}
    .skills{display:flex;flex-wrap:wrap;gap:8px}
    .skill{background:rgba(255,255,255,0.03);padding:8px 10px;border-radius:999px;font-size:13px;color:#eaeaea}

    /* CTA button */
    .btn{
      display:inline-block;padding:12px 18px;border-radius:999px;font-weight:700;text-decoration:none;
      background:linear-gradient(90deg,var(--accent1),var(--accent2));
      color:white;margin-top:14px;box-shadow:0 8px 18px rgba(0,102,255,0.12);
    }
    .btn:active{transform:translateY(1px)}

    footer{margin-top:18px;color:var(--muted);font-size:13px}

    /* small helper */
    .muted{color:var(--muted);font-size:13px}
    .divider{height:1px;background:rgba(255,255,255,0.04);margin:14px 0;border-radius:2px}

    /* top-right controls */
    .top-actions{display:flex;gap:8px;position:absolute;right:12px;top:12px}
    .icon-btn{background:rgba(0,0,0,0.25);padding:8px;border-radius:8px;cursor:pointer;border:1px solid rgba(255,255,255,0.02)}
    .icon-btn:hover{transform:translateY(-2px)}

    /* light mode support
