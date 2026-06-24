# Thapar Grade Predictor

A production-ready grade prediction platform for Thapar Institute of Engineering and Technology students. Predicts student grades based on percentile ranking and comparative performance analysis.

![Build Status](https://img.shields.io/badge/status-production--ready-green)
![License](https://img.shields.io/badge/license-proprietary-red)
![Next.js](https://img.shields.io/badge/Next.js-16-black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.7-blue)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-green)

## Features

### Student Features
- ✅ Secure Google OAuth authentication (Thapar domain restricted)
- ✅ One-time marks submission per subject
- ✅ Grade prediction based on percentile ranking
- ✅ Historical grade boundaries fallback
- ✅ Real-time statistics and analytics
- ✅ Comparative performance analysis
- ✅ Internal marks breakdown tracking
- ✅ Edit request workflow for mark modifications
- ✅ In-app notifications and email alerts
- ✅ Detailed statistical visualizations

### Admin Features
- ✅ Subject and curriculum management
- ✅ Grade cutoff configuration
- ✅ Edit request approval/rejection
- ✅ User account management
- ✅ System-wide analytics dashboard
- ✅ Comprehensive audit logging
- ✅ Data export (CSV, Excel, PDF)
- ✅ Statistics caching and optimization

### Technical Features
- ✅ Multi-role access control
- ✅ Audit trail logging
- ✅ Advanced grade prediction engine
- ✅ Statistical analysis (median, mode, std dev, percentiles)
- ✅ Responsive design (mobile-first)
- ✅ Ancient parchment academic theme
- ✅ Real-time data visualization with Recharts
- ✅ RESTful API with validation

## Tech Stack

### Frontend
- **Framework**: Next.js 16 with App Router
- **Language**: TypeScript 5.7
- **UI Framework**: ShadCN UI
- **Styling**: Tailwind CSS v4
- **State Management**: SWR for data fetching
- **Charts**: Recharts
- **Authentication**: NextAuth.js
- **Fonts**: Playfair Display (headings), Crimson Text (body)

### Backend
- **Runtime**: Node.js 18+
- **Framework**: Next.js 16 (Route Handlers)
- **Database**: MongoDB Atlas
- **ORM**: Prisma
- **Validation**: Zod
- **Authentication**: NextAuth.js with Google OAuth

### DevOps
- **Hosting**: Vercel (Frontend + API)
- **Database Hosting**: MongoDB Atlas
- **Package Manager**: pnpm

## Database Schema

### Core Models
- **User**: Students and admins
- **Subject**: Courses/subjects
- **Semester**: Academic periods
- **Mark**: Mark submissions (unique per student-subject)
- **Statistics**: Cached statistics per subject
- **HistoricalCutoff**: Grade boundaries per subject
- **EditRequest**: Mark modification workflow
- **EditHistory**: Audit trail for mark changes
- **Notification**: User notifications
- **AuditLog**: System audit trail

## Grade Prediction Algorithm

### Percentile-Based Prediction (When ≥100 submissions)

### Historical Cutoff Fallback (When <100 submissions)

## API Endpoints

### Authentication
- `GET/POST /api/auth/[...nextauth]` - NextAuth routes

### Public
- `GET /api/subjects` - List active subjects

### Student
- `GET /api/student/marks` - Get student marks
- `POST /api/student/marks` - Submit marks
- `GET /api/student/statistics/[subjectId]` - Get subject statistics
- `POST /api/student/marks/[id]/edit-request` - Request mark edit


## Performance Optimization

### Implemented
- [x] SWR caching with revalidation
- [x] Prisma query optimization
- [x] Database indexing on frequently queried fields
- [x] CSS optimization with Tailwind
- [x] Image optimization
- [x] Statistics caching

## Security

### Implemented
- ✅ Domain-restricted authentication (@thapar.edu)
- ✅ JWT session management
- ✅ HTTPS/TLS enforced
- ✅ CSRF protection via NextAuth
- ✅ Input validation with Zod
- ✅ Row-level access control
- ✅ Comprehensive audit logging
- ✅ Secure password handling

## Support

For issues or questions: email: aphophalia_be24@thapar.edu

## Version History

### v1.0.0 (Current)
- Initial production release
- Complete authentication system
- Grade prediction engine
- Analytics and visualization
- Admin dashboard
- Audit logging

---

**Last Updated**: June 2026
**Maintained By**: Anirudh Phophalia
**Status**: Under Development
