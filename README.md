<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>URGG - Prototipo App Móvil</title>
    <style>
        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif; background-color: #f1f5f9; color: #1e293b; padding: 20px; display: flex; flex-direction: column; align-items: center; min-height: 100vh; }
        .app-container { background-color: #ffffff; width: 100%; max-width: 400px; border-radius: 20px; box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.1); overflow: hidden; border: 1px solid #e2e8f0; }
        .app-header { background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%); color: #ffffff; padding: 30px 20px; text-align: center; }
        .app-header h1 { font-size: 22px; font-weight: 700; margin-bottom: 5px; letter-spacing: 0.5px; }
        .app-header p { font-size: 13px; opacity: 0.9; }
        .app-content { padding: 25px 20px; }
        .section-title { font-size: 14px; font-weight: 600; text-transform: uppercase; color: #64748b; letter-spacing: 1px; margin-bottom: 15px; }
        .menu-link { display: flex; align-items: center; background-color: #f8fafc; border: 1px solid #e2e8f0; padding: 16px; border-radius: 12px; text-decoration: none; color: #334155; margin-bottom: 16px; transition: all 0.2s ease; }
        .menu-link:hover { background-color: #f1f5f9; transform: translateY(-1px); border-color: #cbd5e1; }
        .icon { font-size: 24px; margin-right: 15px; width: 35px; text-align: center; }
        .text-container { display: flex; flex-direction: column; }
        .link-title { font-size: 16px; font-weight: 600; color: #0f172a; }
        .link-desc { font-size: 12px; color: #64748b; margin-top: 2px; }
        .btn-excel { border-left: 4px solid #16a34a; }
        .btn-pdf { border-left: 4px solid #dc2626; }
        .app-footer { text-align: center; padding: 15px; font-size: 11px; color: #94a3b8; background-color: #f8fafc; border-top: 1px solid #e2e8f0; }
    </style>
</head>
<body>

    <div class="app-container">
        <!-- Encabezado de la App -->
        <div class="app-header">
            <h1>URGG Prototipo</h1>
            <p>Panel de Gestión de Inventario Móvil</p>
        </div>

        <!-- Contenido Principal -->
        <div class="app-content">
            <p class="section-title">Accesos Directos</p>

            <!-- ENLACE AL EXCEL DE INVENTARIO -->
            <a href="URGG_inventario_QR_base.xlsx" download class="menu-link btn-excel">
                <span class="icon">📊</span>
                <div class="text-container">
                    <span class="link-title">Base de Datos Excel</span>
                    <span class="link-desc">Descargar URGG_inventario_QR_base</span>
                </div>
            </a>

            <!-- ENLACE AL PDF DE ETIQUETAS -->
            <a href="URGG_QR_piloto_24_etiquetas.pdf" target="_blank" class="menu-link btn-pdf">
                <span class="icon">📄</span>
                <div class="text-container">
                    <span class="link-title">Piloto 24 Etiquetas QR</span>
                    <span class="link-desc">Ver documento de impresión PDF</span>
                </div>
            </a>
        </div>

        <!-- Pie de página de la App -->
        <div class="app-footer">
            URGG_AppMovil_Prototipo &copy; 2026
        </div>
    </div>

</body>
</html>
