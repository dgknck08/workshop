# workshop
### PostgreSQL Tabloları
```sql
-- Kullanıcılar
users (id, username, email, password_hash, first_name, last_name, role, created_at, updated_at)

-- Etkinlikler
events (id, title, description, organizer_id, category, location, start_date, end_date, 
        capacity, price, status, created_at, updated_at)

-- Biletler/Kayıtlar
registrations (id, user_id, event_id, status, registration_date, payment_status, ticket_code)

-- Ödemeler
payments (id, registration_id, amount, payment_method, status, transaction_id, created_at)

-- Değerlendirmeler
ratings (id, user_id, event_id, rating, created_at)
```

### MongoDB Collections
```javascript
// Yorumlar
comments: {
  _id, userId, eventId, content, parentCommentId, 
  likes: [], createdAt, updatedAt
}

// Sistem Logları
system_logs: {
  _id, level, message, userId, eventId, metadata, timestamp
}
```

### week 1: Temel  
- [ ] Spring Boot projesi kurulumu
- [ ] Docker Compose ile PostgreSQL, Redis, MongoDB
- [ ] Temel entity'ler ve repository'ler
- [ ] Database migration (Flyway/Liquibase)
- [ ] Basic logging configuration

