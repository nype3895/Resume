[Nylah Perry - Ulta Beauty Resume.docx](https://github.com/user-attachments/files/18791548/Nylah.Perry.-.Ulta.Beauty.Resume.docx)
import React, { useState } from 'react';
import { User, Medal, Camera, Briefcase, GraduationCap, Instagram, Mail, Phone, Sun, Moon } from 'lucide-react';
import { Switch } from '@/components/ui/switch';

const Portfolio = () => {
  const [activeSection, setActiveSection] = useState('about');
  const [isDarkMode, setIsDarkMode] = useState(true);

  const NavigationItem = ({ section, icon: Icon, label }) => (
    <button
      onClick={() => setActiveSection(section)}
      className={`flex items-center gap-2 px-4 py-2 rounded-lg transition-all
        ${activeSection === section 
          ? 'bg-purple-600 text-white' 
          : isDarkMode 
            ? 'hover:bg-gray-800 text-gray-300' 
            : 'hover:bg-gray-100 text-gray-700'}`}
    >
      <Icon size={20} />
      <span>{label}</span>
    </button>
  );

  return (
    <div className={`min-h-screen transition-colors duration-200 ${
      isDarkMode ? 'bg-gray-900 text-gray-100' : 'bg-gray-50 text-gray-900'
    }`}>
      {/* Theme Toggle */}
      <div className="absolute top-4 right-4 flex items-center gap-2">
        <Sun size={20} className={isDarkMode ? 'text-gray-500' : 'text-yellow-500'} />
        <Switch
          checked={isDarkMode}
          onCheckedChange={setIsDarkMode}
        />
        <Moon size={20} className={isDarkMode ? 'text-blue-400' : 'text-gray-500'} />
      </div>

      {/* Hero Section */}
      <div className={`bg-gradient-to-r ${
        isDarkMode 
          ? 'from-purple-900 to-blue-900' 
          : 'from-purple-600 to-blue-500'
      } text-white`}>
        <div className="container mx-auto px-4 py-16">
          <div className="flex flex-col items-center text-center">
            <div className="w-32 h-32 rounded-full bg-white/20 mb-6 flex items-center justify-center">
              <User size={48} />
            </div>
            <h1 className="text-4xl font-bold mb-2">Nylah Perry</h1>
            <p className="text-xl mb-4">Strategic Communication Designer & Athlete</p>
            <div className="flex gap-4">
              <a href="mailto:nylahperry24@gmail.com" className="flex items-center gap-2 hover:text-purple-200">
                <Mail size={20} />
                <span>Email</span>
              </a>
              <a href="tel:8564191858" className="flex items-center gap-2 hover:text-purple-200">
                <Phone size={20} />
                <span>Call</span>
              </a>
              <a href="#" className="flex items-center gap-2 hover:text-purple-200">
                <Instagram size={20} />
                <span>87k followers</span>
              </a>
            </div>
          </div>
        </div>
      </div>

      {/* Main Content */}
      <div className="container mx-auto px-4 py-8">
        <nav className="flex gap-4 mb-8 overflow-x-auto">
          <NavigationItem section="about" icon={User} label="About" />
          <NavigationItem section="experience" icon={Briefcase} label="Experience" />
          <NavigationItem section="athletics" icon={Medal} label="Athletics" />
          <NavigationItem section="education" icon={GraduationCap} label="Education" />
          <NavigationItem section="content" icon={Camera} label="Content Creation" />
        </nav>

        <div className="grid md:grid-cols-3 gap-8">
          {/* Main Content Area */}
          <div className="md:col-span-2 space-y-8">
            {activeSection === 'about' && (
              <div className={`p-6 rounded-lg shadow-sm ${
                isDarkMode ? 'bg-gray-800' : 'bg-white'
              }`}>
                <h2 className="text-2xl font-bold mb-4">About Me</h2>
                <p className={`mb-4 ${isDarkMode ? 'text-gray-300' : 'text-gray-600'}`}>
                  I'm a Strategic Communication Design graduate student at the University of Colorado Boulder, 
                  combining my passion for athletics with creative digital communication. As a Division I athlete 
                  and content creator with over 200k combined followers, I bring a unique perspective to strategic 
                  communication and digital marketing.
                </p>
                <div className="grid grid-cols-2 gap-4">
                  <div className={`p-4 rounded-lg ${
                    isDarkMode ? 'bg-gray-700' : 'bg-gray-50'
                  }`}>
                    <h3 className="font-bold mb-2">Content Creation</h3>
                    <p className={isDarkMode ? 'text-gray-300' : 'text-gray-600'}>120k+ TikTok followers</p>
                    <p className={isDarkMode ? 'text-gray-300' : 'text-gray-600'}>87k+ Instagram followers</p>
                  </div>
                  <div className={`p-4 rounded-lg ${
                    isDarkMode ? 'bg-gray-700' : 'bg-gray-50'
                  }`}>
                    <h3 className="font-bold mb-2">Athletics</h3>
                    <p className={isDarkMode ? 'text-gray-300' : 'text-gray-600'}>Division I Track Athlete</p>
                    <p className={isDarkMode ? 'text-gray-300' : 'text-gray-600'}>Academic All-Big Ten</p>
                  </div>
                </div>
              </div>
            )}

            {activeSection === 'experience' && (
              <div className="space-y-6">
                {[
                  {
                    title: "Digital Marketing Intern",
                    company: "Mural Arts of Philadelphia",
                    date: "June 2024 - August 2024",
                    points: [
                      "Created digital assets for 40th-anniversary campaign",
                      "Led production of engaging social media content",
                      "Collaborated with cross-functional teams"
                    ]
                  },
                  {
                    title: "Creative Developer",
                    company: "Golden Herky Award Show",
                    date: "April 2022 - May 2024",
                    points: [
                      "Coordinated makeup and styling for event hosts",
                      "Directed visual aspects of the award show"
                    ]
                  },
                  {
                    title: "Front Desk Associate",
                    company: "City Fitness",
                    date: "June 2023 - December 2024",
                    points: [
                      "Delivered outstanding guest service",
                      "Guided members through account management"
                    ]
                  }
                ].map((job, index) => (
                  <div key={index} className={`p-6 rounded-lg shadow-sm ${
                    isDarkMode ? 'bg-gray-800' : 'bg-white'
                  }`}>
                    <h3 className="text-xl font-bold mb-2">{job.title}</h3>
                    <p className={`mb-2 ${
                      isDarkMode ? 'text-gray-400' : 'text-gray-500'
                    }`}>{job.company} | {job.date}</p>
                    <ul className={`list-disc list-inside space-y-2 ${
                      isDarkMode ? 'text-gray-300' : 'text-gray-600'
                    }`}>
                      {job.points.map((point, i) => (
                        <li key={i}>{point}</li>
                      ))}
                    </ul>
                  </div>
                ))}
              </div>
            )}

            {/* Other sections would follow the same pattern - omitted for brevity */}
          </div>

          {/* Sidebar */}
          <div className="space-y-6">
            <div className={`p-6 rounded-lg shadow-sm ${
              isDarkMode ? 'bg-gray-800' : 'bg-white'
            }`}>
              <h3 className="font-bold mb-4">Skills</h3>
              <div className="space-y-2">
                {[
                  "Adobe Illustrator",
                  "Adobe Photoshop",
                  "Social Media Management",
                  "Content Creation",
                  "Digital Marketing",
                  "Event Planning"
                ].map((skill, index) => (
                  <div key={index} className={`p-2 rounded ${
                    isDarkMode 
                      ? 'bg-purple-900/50 text-purple-200' 
                      : 'bg-purple-100 text-purple-700'
                  }`}>
                    {skill}
                  </div>
                ))}
              </div>
            </div>

            <div className={`p-6 rounded-lg shadow-sm ${
              isDarkMode ? 'bg-gray-800' : 'bg-white'
            }`}>
              <h3 className="font-bold mb-4">Leadership Roles</h3>
              <div className="space-y-4">
                <div>
                  <h4 className="font-semibold">BSAA Secretary</h4>
                  <p className={isDarkMode ? 'text-gray-400' : 'text-gray-600'}>
                    Black Student Athlete Alliance
                  </p>
                </div>
                <div>
                  <h4 className="font-semibold">ISAAC Member</h4>
                  <p className={isDarkMode ? 'text-gray-400' : 'text-gray-600'}>
                    Iowa Student-Athlete Advisory Committee
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
};

export default Portfolio;
