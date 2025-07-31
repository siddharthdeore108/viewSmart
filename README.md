// 📁 Project: Real Estate QR Platform

// ✅ Tech Stack
// - Frontend: Next.js (React)
// - Backend: Supabase (DB, Auth, Storage)
// - Analytics: PostHog

// ✅ Folder Structure

/app
  /builder
    - dashboard.tsx            // Builder Admin Panel
    - add-project.tsx         // Upload new LOD200 model + details
  /viewer
    - [builderId].tsx         // Public QR-based project viewer
  /project
    - [projectId].tsx         // Individual project page with VR/info
  /api
    - submit-lead.ts          // Lead capture handler

/components
  - MapViewer.tsx             // 3D Map viewer using Three.js/Mapbox
  - ProjectCard.tsx           // Project overview card
  - LeadForm.tsx              // Form to submit buyer/vendor interest

/lib
  - supabase.ts               // Supabase client init
  - posthog.ts                // PostHog event tracking

/styles
  - globals.css               // Tailwind or custom

/utils
  - modelUploader.ts          // Convert .skp/.glb to viewer format

/public
  - placeholder models/images

.env
  - SUPABASE_URL
  - SUPABASE_KEY
  - POSTHOG_KEY

// ✅ Key Dev Goals
// - MVP: QR opens 3D map, project cards, lead form
// - Supabase: auth, file storage, DB (projects, leads)
// - PostHog: basic funnel + feedback tracking

// ✅ Dev Scripts
// npm run dev: local dev
// npm run build: production
// vercel deploy: Vercel deployment

// Start small, iterate fast 💪
