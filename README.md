import React from 'react';
import { Github, Linkedin, Twitter, Mail } from 'lucide-react';

const GithubProfile = () => {
  return (
    <div className="max-w-4xl mx-auto p-8 space-y-8 bg-gradient-to-br from-gray-900 to-gray-800 text-white rounded-lg">
      {/* Header Section */}
      <div className="text-center space-y-4">
        <h1 className="text-4xl font-bold bg-gradient-to-r from-blue-400 to-purple-500 bg-clip-text text-transparent">
          Goodness Mbakara
        </h1>
        <p className="text-xl text-gray-300">
          Backend Engineer | FOCOSA President | Passionate About Scalable Systems
        </p>
      </div>

      {/* About Section */}
      <div className="grid md:grid-cols-2 gap-8">
        <div className="space-y-4">
          <h2 className="text-2xl font-semibold text-blue-400">🚀 About Me</h2>
          <ul className="space-y-2 text-gray-300">
            <li className="flex items-center space-x-2">
              <span className="text-blue-400">•</span>
              <span>President, Faculty of Computing Students Association (FOCOSA), University of Uyo</span>
            </li>
            <li className="flex items-center space-x-2">
              <span className="text-blue-400">•</span>
              <span>Backend Engineer at Kwekmarket.com</span>
            </li>
            <li className="flex items-center space-x-2">
              <span className="text-blue-400">•</span>
              <span>Optimizing performance & scalability with Python benchmarking</span>
            </li>
          </ul>
        </div>
        
        <div className="relative">
          <div className="absolute inset-0 bg-gradient-to-r from-blue-500/20 to-purple-500/20 rounded-lg filter blur-xl"></div>
          <div className="relative bg-gray-800 p-6 rounded-lg border border-gray-700">
            <h2 className="text-2xl font-semibold text-blue-400 mb-4">🔧 Tech Stack</h2>
            <div className="grid grid-cols-4 gap-4">
              {['Python', 'JavaScript', 'TypeScript', 'Docker', 'Linux', 'MySQL', 'PostgreSQL', 'Django'].map((tech) => (
                <div key={tech} className="flex items-center justify-center p-2 bg-gray-700 rounded-lg hover:bg-gray-600 transition-colors">
                  <span className="text-sm">{tech}</span>
                </div>
              ))}
            </div>
          </div>
        </div>
      </div>

      {/* Stats Section */}
      <div className="grid md:grid-cols-3 gap-4">
        {['Contributions', 'Projects', 'Pull Requests'].map((stat, index) => (
          <div key={stat} className="bg-gray-800 p-6 rounded-lg border border-gray-700 text-center">
            <h3 className="text-xl font-semibold text-blue-400">{stat}</h3>
            <p className="text-3xl font-bold mt-2 text-gray-300">{(index + 1) * 127}</p>
          </div>
        ))}
      </div>

      {/* Connect Section */}
      <div className="space-y-4">
        <h2 className="text-2xl font-semibold text-blue-400">🔗 Connect with Me</h2>
        <div className="flex space-x-4">
          <a href="https://github.com/Goodnessmbakara" className="p-2 bg-gray-800 rounded-lg hover:bg-gray-700 transition-colors">
            <Github className="w-6 h-6" />
          </a>
          <a href="https://linkedin.com/in/goodnessmbakara" className="p-2 bg-gray-800 rounded-lg hover:bg-gray-700 transition-colors">
            <Linkedin className="w-6 h-6" />
          </a>
          <a href="https://twitter.com/Goodnessmbakara" className="p-2 bg-gray-800 rounded-lg hover:bg-gray-700 transition-colors">
            <Twitter className="w-6 h-6" />
          </a>
          <a href="mailto:mbakaragoodness2003@gmail.com" className="p-2 bg-gray-800 rounded-lg hover:bg-gray-700 transition-colors">
            <Mail className="w-6 h-6" />
          </a>
        </div>
      </div>

      <div className="text-center text-gray-400 mt-8">
        <p>💡 Let's Build Something Amazing Together 🚀</p>
      </div>
    </div>
  );
};

export default GithubProfile;
