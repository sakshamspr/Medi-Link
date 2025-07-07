# Medi-Link: Hospital & Doctor Appointment Finder

A modern web application that helps users **find nearby hospitals and book doctor appointments** based on their location. The platform provides an intuitive map interface, specialty-based search, and real-time email confirmations upon appointment booking.

## Features

- **Location-based Hospital & Doctor Search**: Find hospitals and doctors near your current location
- **Doctor Appointment Booking**: Users can view available slots and book appointments directly
- **Email Confirmation**: Patients receive a confirmation email after booking
- **Interactive Map**: Visual representation of hospital locations with custom markers
- **Customizable Search Radius**: Select search radius from 1km to 25km
- **Detailed Hospital and Doctor Information**: View names, addresses, distances, and specialties
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Real-time Results**: Dynamic updates based on your selected criteria

## Technologies Used

- **Frontend**: React 18 with TypeScript
- **Styling**: Tailwind CSS
- **UI Components**: shadcn/ui component library
- **Build Tool**: Vite
- **Maps & Location**: Geoapify API
- **Icons**: Lucide React
- **State Management**: React Query (@tanstack/react-query)
- **Backend Services**: Supabase (PostgreSQL)
- **Email Service**: Email API (e.g., EmailJS or NodeMailer)

## Screenshots
![Homepage](https://github.com/user-attachments/assets/d1d4e95a-13f5-4b43-a351-70e099bc2a92)
![Doctor List](https://github.com/user-attachments/assets/631dba50-2f3d-4f45-8efd-947d8e362efd)
![Appointment Booking](https://github.com/user-attachments/assets/45cae80d-d731-4434-a669-7d223f27047d)
![Mobile View](https://github.com/user-attachments/assets/38eaf41e-17ac-4a5b-a03e-3a387eb9a476)

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn package manager

### Installation

```bash
git clone <your-repository-url>
cd hospital-finder
npm install
```

### Development

```bash
npm run dev
```

Visit: `http://localhost:5173`

### Configuration

- **Geoapify API**: For maps and hospital data
  - Get your API key from [Geoapify](https://www.geoapify.com/)
  - Replace the key in the `HospitalMap` component
- **Supabase**: For storing doctors, appointments, and users
- **Email**: Set up email API (like EmailJS or Nodemailer) for sending confirmation

## Project Structure

```
src/
├── components/
│   ├── ui/
│   ├── HospitalMap.tsx       # Map with markers
│   ├── HospitalList.tsx      # List of hospitals
│   ├── DoctorList.tsx        # List of doctors
│   └── AppointmentForm.tsx   # Form to book appointment
├── pages/
│   └── Book.tsx              # Main appointment booking page
├── hooks/                    # Custom hooks
├── lib/                      # Utility functions
└── integrations/             # API calls & Supabase logic
```

## Key Features

### 🏥 Hospital Finder
- Search by location and radius
- See results on map and list view

### 👨‍⚕️ Doctor Appointment
- Filter by specialty
- Book appointment from available slots
- Stores appointments on Supabase

### 📧 Email Notification
- Sends confirmation email to user after booking
- Integration with external email service provider

## Usage

1. **Allow Location Access** when prompted
2. **Select Search Radius**
3. **View Hospitals & Doctors**
4. **Book Appointment**
5. **Receive Email Confirmation**

## API Integration

- **Geoapify**: Geocoding, reverse geocoding, places search
- **Supabase**: Doctor and appointment data (PostgreSQL)
- **Email API**: Confirmation messages

## Build and Deployment

### Development
```bash
npm run dev
```

### Production
```bash
npm run build
npm run preview
```

Deploy `/dist` to any static host (Vercel, Netlify, etc.)

## Browser Support

- Chrome
- Firefox
- Safari
- Edge

## Contributing

```bash
git checkout -b feature/your-feature
git commit -m "Add feature"
git push origin feature/your-feature
```

Then open a Pull Request

## Acknowledgments

- [Geoapify](https://www.geoapify.com/)
- [Supabase](https://supabase.com/)
- [Tailwind CSS](https://tailwindcss.com/)
- [shadcn/ui](https://ui.shadcn.com/)
- [React](https://reactjs.org/)
- [Lucide Icons](https://lucide.dev/)
