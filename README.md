Project Name: Fitness Studio


Here's what I built and why each design decision was made:

Visual Identity:
- Neon orange (#FF5E00) as the primary accent — aggressive, energetic, impossible to ignore
- Metallic silver for secondary text — adds that premium, industrial feel without competing with orange
- High-contrast B&W photography via CSS `grayscale(100%) contrast(1.3)` filters that reveal color on hover
- Textured dark backgrounds using a noise SVG overlay for depth and tactile quality

Key Interactive Features:
- Functional weekly schedule with day-by-day tab switching, showing real class data with spots remaining
- Booking form with loading state, success confirmation, and toast notification — no `alert()` calls
- Mobile hamburger menu with smooth slide-in animation and overlay
- Scroll-triggered card animations using IntersectionObserver

Typography Strategy:
- Oswald for all headings — condensed, powerful, space-efficient
- Inter for body text — clean legibility at small sizes
- Minimal spacing, high information density as requested

Content Architecture:
1. Hero — brand attitude statement + embedded coach showcase
2. Programs — goal-oriented cards (Muscle Gain, Fat Loss, Total Fitness) with pricing
3. Coaches — 4 profiles with certifications and specialties
4. Schedule — interactive weekly timetable
5. Member Stories — before/after transformation cards with real metrics
6. Book Trial — full form with social proof and trust indicators


1. Technology Stack:
Technology	      কাজ
HTML5	            Structure
Tailwind CSS	    Styling (CDN থেকে)
Iconify	Icons     (Lucide icons)
Google Fonts	    Oswald + Inter fonts
JavaScript	      Interactivity

2. Project Structure (Step by Step):
🔷 Head Section (Lines 1-50)
Tailwind CDN - CSS Framework লোড
Iconify - Icon library
Google Fonts - Oswald (heading) + Inter (body)
Custom Colors - forge-black, forge-orange etc. Tailwind config এ define করা
Custom Animations - fadeInUp, pulse-glow, marquee ইত্যাদি

🔷 CSS Styles (Lines 51-200)
Texture overlay (noise effect)
Custom scrollbar (orange color)
Hero image grayscale filter
Coach card hover effects
Mobile menu transition
Form input focus effects

🔷 Navigation (Lines 203-280)
Fixed navbar with blur effect
Logo + Desktop menu links
"Book Trial" CTA button
Mobile hamburger menu
Mobile slide-in menu panel

🔷 Hero Section (Lines 283-400)
Full-screen background image
Gradient overlays
Main headline: "Break Your Limits"
Stats: 2,400+ Members, 98% Goal Achievement, 15+ Coaches
CTA buttons
Coach thumbnails with availability indicator

🔷 Marquee Banner (Lines 403-430)
Infinite scrolling text (CSS animation)
Training programs list

🔷 Programs Section (Lines 433-560)
3 Program Cards:
Muscle Gain - $199/month
Fat Loss - $179/month (Most Popular badge)
Total Fitness - $149/month
Quick info bar (duration, coach ratio, InBody scan, nutrition)

🔷 Coaches Section (Lines 563-720)
4 Coach Cards with:
Profile images
Hover effects (social icons appear)
Certifications
Experience years
Specializations

🔷 Schedule Section (Lines 723-780)
Day tabs (Mon-Sun)
JavaScript দিয়ে dynamic class schedule load হয়
Class info: time, name, coach, level, spots left

🔷 Member Stories Section (Lines 783-920)
Before/After comparison images
Member testimonials
Results achieved (weight loss/gain)

🔷 Book Trial Section (Lines 923-1070)
Free trial offer
Benefits list
Trust indicators (reviews)
Booking form with:
Name, Email, Phone
Goal dropdown
Experience level (radio buttons)
Submit button with loading state

🔷 Contact Section (Lines 1073-1140)
Address
Operating Hours
Phone/Email
Social media links

🔷 Footer (Lines 1143-1170)
Logo
Copyright
Privacy/Terms links

3. JavaScript Features
Feature	            কিভাবে কাজ করে
Mobile Menu	        Toggle class + overlay
Navbar Scroll	      Border appears on scroll
Schedule Tabs	      Dynamic content rendering
Form Submit	        Loading state → Success message
Toast Notifications	Success/error popups
Scroll Animations	  IntersectionObserver দিয়ে fade-in

4. Design Highlights
Dark Theme - Black (#0A0A0A) base
Orange Accent - #FF5E00 for CTAs and highlights
Typography - Bold headings (Oswald), clean body (Inter)
Grayscale Images - Hover করলে color আসে
Smooth Animations - CSS transitions + keyframes

