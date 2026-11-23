# Esquema Supabase (proyecto lsenowftafzotgofcqjo)
Tablas: profiles, catalog_products, orders, order_items, order_status_history (RLS activo).
RPC: create_distributor_order(p_items, p_requested_delivery_date, p_delivery_address, p_notes).
Regla vigente: sin pedido mínimo; envío fijo de $12.000; alimento cocido = PVP x (1 - descuento del perfil); complementos = precio mayorista.
Alta de distribuidor: crear usuario en Auth y luego insertar su fila en profiles (id = auth.users.id, role='distributor', discount_level 15|18|20).
