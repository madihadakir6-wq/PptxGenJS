import React, { useState } from 'react';
import { ChevronLeft, ChevronRight, Users, Target, Lightbulb, TrendingUp, Award, CheckCircle } from 'lucide-react';

const Presentation = () => {
  const [currentSlide, setCurrentSlide] = useState(0);

  const slides = [
    {
      type: 'title',
      content: (
        <div className="flex flex-col items-center justify-center h-full bg-gradient-to-br from-purple-600 via-pink-500 to-orange-500 text-white relative overflow-hidden">
          <div className="absolute inset-0 opacity-20">
            <div className="absolute top-10 left-10 w-72 h-72 bg-yellow-300 rounded-full blur-3xl"></div>
            <div className="absolute bottom-20 right-20 w-96 h-96 bg-blue-400 rounded-full blur-3xl"></div>
          </div>
          <div className="text-center space-y-6 z-10">
            <div className="inline-block p-6 bg-white/20 rounded-3xl backdrop-blur-lg mb-6 shadow-2xl border-4 border-white/30">
              <div className="w-28 h-28 bg-gradient-to-br from-yellow-300 via-orange-400 to-pink-500 rounded-2xl flex items-center justify-center shadow-xl">
                <TrendingUp className="w-16 h-16 text-white" />
              </div>
            </div>
            <h1 className="text-8xl font-black mb-6 drop-shadow-2xl">MEDIA 311 PRO</h1>
            <p className="text-4xl font-bold tracking-wide drop-shadow-lg">LET'S GROW TOGETHER</p>
            <div className="mt-16 text-2xl font-semibold bg-white/20 px-8 py-4 rounded-full backdrop-blur-md border-2 border-white/30 inline-block">
              Agence de Marketing Numérique
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-blue-400 via-purple-400 to-pink-400 p-16">
          <h1 className="text-6xl font-black mb-12 text-white drop-shadow-lg">Notre Agence de Marketing Numérique</h1>
          <div className="space-y-8">
            <div className="bg-white/95 backdrop-blur-lg p-10 rounded-3xl shadow-2xl border-4 border-yellow-300">
              <p className="text-3xl text-gray-800 leading-relaxed font-semibold">
                Bonjour à tous ! Nous sommes l'équipe MEDIA 311 PRO et notre objectif est de créer une agence de marketing numérique spécialisée pour les PME.
              </p>
            </div>
            <div className="grid grid-cols-3 gap-6">
              <div className="bg-gradient-to-br from-green-400 to-emerald-600 p-8 rounded-2xl shadow-2xl transform hover:scale-105 transition-transform border-4 border-white">
                <Users className="w-16 h-16 text-white mb-4 drop-shadow-lg" />
                <h3 className="font-black text-3xl mb-2 text-white">16 Membres</h3>
                <p className="text-white text-xl font-semibold">Équipe complète</p>
              </div>
              <div className="bg-gradient-to-br from-orange-400 to-red-600 p-8 rounded-2xl shadow-2xl transform hover:scale-105 transition-transform border-4 border-white">
                <Target className="w-16 h-16 text-white mb-4 drop-shadow-lg" />
                <h3 className="font-black text-3xl mb-2 text-white">PME</h3>
                <p className="text-white text-xl font-semibold">Notre cible</p>
              </div>
              <div className="bg-gradient-to-br from-yellow-400 to-orange-600 p-8 rounded-2xl shadow-2xl transform hover:scale-105 transition-transform border-4 border-white">
                <Award className="w-16 h-16 text-white mb-4 drop-shadow-lg" />
                <h3 className="font-black text-3xl mb-2 text-white">Excellence</h3>
                <p className="text-white text-xl font-semibold">Notre engagement</p>
              </div>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-indigo-500 via-purple-500 to-pink-500 p-16">
          <h1 className="text-6xl font-black mb-10 text-white drop-shadow-lg">Présentation de l'Équipe</h1>
          <p className="text-2xl text-white mb-8 font-semibold drop-shadow-md">Notre équipe de 16 membres aux rôles complémentaires</p>
          <div className="grid grid-cols-2 gap-6">
            <div className="bg-gradient-to-br from-red-400 to-pink-600 p-7 rounded-2xl shadow-2xl border-4 border-white transform hover:scale-105 transition-transform">
              <h3 className="font-black text-2xl text-white mb-3">📢 Annonce & Campagnes</h3>
              <p className="text-xl text-white font-semibold">Soumiya Essoualh, Anas Soultani</p>
            </div>
            <div className="bg-gradient-to-br from-green-400 to-emerald-600 p-7 rounded-2xl shadow-2xl border-4 border-white transform hover:scale-105 transition-transform">
              <h3 className="font-black text-2xl text-white mb-3">📊 Reporting & Analyse</h3>
              <p className="text-xl text-white font-semibold">Maryam Moumni, Maria Nejmessabah, Hayat Hasni</p>
            </div>
            <div className="bg-gradient-to-br from-blue-400 to-cyan-600 p-7 rounded-2xl shadow-2xl border-4 border-white transform hover:scale-105 transition-transform">
              <h3 className="font-black text-2xl text-white mb-3">💬 Communication Interne</h3>
              <p className="text-xl text-white font-semibold">Rida Mohamed, Mohammed El Siki, Rachid Harbachi</p>
            </div>
            <div className="bg-gradient-to-br from-purple-400 to-indigo-600 p-7 rounded-2xl shadow-2xl border-4 border-white transform hover:scale-105 transition-transform">
              <h3 className="font-black text-2xl text-white mb-3">✍️ Contenu & Copywriting</h3>
              <p className="text-xl text-white font-semibold">Fatima-ezzahra Khalil, Madiha Dakir, Jamal Elkahia</p>
            </div>
            <div className="bg-gradient-to-br from-pink-400 to-rose-600 p-7 rounded-2xl shadow-2xl border-4 border-white transform hover:scale-105 transition-transform">
              <h3 className="font-black text-2xl text-white mb-3">🎨 Design</h3>
              <p className="text-xl text-white font-semibold">Youssef Lhrizi, Youssef Titaou, Naima Benrais</p>
            </div>
            <div className="bg-gradient-to-br from-yellow-400 to-orange-600 p-7 rounded-2xl shadow-2xl border-4 border-white transform hover:scale-105 transition-transform">
              <h3 className="font-black text-2xl text-white mb-3">📅 Organisation & Deadlines</h3>
              <p className="text-xl text-white font-semibold">Hafida Hamidoun, Rida Mohamed</p>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-red-500 via-orange-500 to-yellow-500 p-16 flex items-center justify-center">
          <div className="max-w-5xl">
            <h1 className="text-6xl font-black mb-12 text-white drop-shadow-lg text-center">Le Problème des PME</h1>
            <div className="bg-white/95 backdrop-blur-lg p-14 rounded-3xl shadow-2xl border-8 border-red-300">
              <div className="flex items-start space-x-8">
                <div className="flex-shrink-0">
                  <div className="w-28 h-28 bg-gradient-to-br from-red-600 to-orange-600 rounded-full flex items-center justify-center shadow-2xl border-4 border-white">
                    <span className="text-6xl">⚠️</span>
                  </div>
                </div>
                <div className="space-y-6">
                  <p className="text-3xl text-gray-800 leading-relaxed font-bold">
                    De nombreuses PME peinent à se développer en ligne, manquant de moyens, de compétences et de stratégie.
                  </p>
                  <p className="text-2xl text-gray-700 font-semibold">
                    Elles dépensent souvent leur budget sans obtenir de résultats concrets.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-cyan-400 via-blue-500 to-indigo-600 p-16">
          <h1 className="text-6xl font-black mb-10 text-white drop-shadow-lg">Notre Solution</h1>
          <p className="text-2xl text-white mb-10 font-semibold drop-shadow-md">Des solutions complètes pour prospérer</p>
          <div className="grid grid-cols-2 gap-8">
            <div className="bg-gradient-to-br from-blue-300 to-blue-600 p-10 rounded-3xl shadow-2xl border-4 border-white">
              <div className="w-20 h-20 bg-white rounded-full flex items-center justify-center mb-6 shadow-xl">
                <span className="text-5xl">📱</span>
              </div>
              <h3 className="font-black text-3xl mb-4 text-white">Gestion Publicitaire</h3>
              <p className="text-white text-xl font-semibold">Facebook, Instagram, Google</p>
            </div>
            <div className="bg-gradient-to-br from-green-300 to-emerald-600 p-10 rounded-3xl shadow-2xl border-4 border-white">
              <div className="w-20 h-20 bg-white rounded-full flex items-center justify-center mb-6 shadow-xl">
                <span className="text-5xl">✨</span>
              </div>
              <h3 className="font-black text-3xl mb-4 text-white">Création de Contenu</h3>
              <p className="text-white text-xl font-semibold">Visuels et textes pros</p>
            </div>
            <div className="bg-gradient-to-br from-purple-300 to-purple-600 p-10 rounded-3xl shadow-2xl border-4 border-white">
              <div className="w-20 h-20 bg-white rounded-full flex items-center justify-center mb-6 shadow-xl">
                <span className="text-5xl">📊</span>
              </div>
              <h3 className="font-black text-3xl mb-4 text-white">Analyse & Reporting</h3>
              <p className="text-white text-xl font-semibold">Suivi des performances</p>
            </div>
            <div className="bg-gradient-to-br from-orange-300 to-red-600 p-10 rounded-3xl shadow-2xl border-4 border-white">
              <div className="w-20 h-20 bg-white rounded-full flex items-center justify-center mb-6 shadow-xl">
                <span className="text-5xl">🎯</span>
              </div>
              <h3 className="font-black text-3xl mb-4 text-white">Stratégies Personnalisées</h3>
              <p className="text-white text-xl font-semibold">Approche sur mesure</p>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-teal-400 via-green-500 to-emerald-600 p-16 flex items-center justify-center">
          <div className="max-w-5xl w-full">
            <h1 className="text-6xl font-black mb-12 text-white drop-shadow-lg text-center">Audience Ciblée</h1>
            <div className="bg-white/95 backdrop-blur-lg p-12 rounded-3xl shadow-2xl border-8 border-green-300">
              <p className="text-2xl text-gray-800 mb-10 font-bold text-center">
                Entrepreneurs locaux, commerçants, freelances et PME en croissance
              </p>
              <div className="grid grid-cols-2 gap-6 mb-10">
                <div className="flex items-center space-x-4 bg-gradient-to-r from-green-400 to-emerald-500 p-6 rounded-2xl shadow-xl border-4 border-white">
                  <CheckCircle className="w-12 h-12 text-white flex-shrink-0" />
                  <span className="text-2xl font-black text-white">Entrepreneurs locaux</span>
                </div>
                <div className="flex items-center space-x-4 bg-gradient-to-r from-blue-400 to-cyan-500 p-6 rounded-2xl shadow-xl border-4 border-white">
                  <CheckCircle className="w-12 h-12 text-white flex-shrink-0" />
                  <span className="text-2xl font-black text-white">Commerçants</span>
                </div>
                <div className="flex items-center space-x-4 bg-gradient-to-r from-purple-400 to-pink-500 p-6 rounded-2xl shadow-xl border-4 border-white">
                  <CheckCircle className="w-12 h-12 text-white flex-shrink-0" />
                  <span className="text-2xl font-black text-white">Freelances</span>
                </div>
                <div className="flex items-center space-x-4 bg-gradient-to-r from-orange-400 to-red-500 p-6 rounded-2xl shadow-xl border-4 border-white">
                  <CheckCircle className="w-12 h-12 text-white flex-shrink-0" />
                  <span className="text-2xl font-black text-white">PME en croissance</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-pink-500 via-purple-500 to-indigo-600 p-16">
          <h1 className="text-6xl font-black mb-10 text-white drop-shadow-lg">Notre Valeur Ajoutée</h1>
          <div className="grid grid-cols-2 gap-10">
            <div className="bg-gradient-to-br from-green-300 to-green-600 p-10 rounded-3xl shadow-2xl text-white border-4 border-white">
              <div className="text-7xl mb-6">💰</div>
              <h3 className="font-black text-4xl mb-4">Prix Accessibles</h3>
              <p className="text-2xl font-semibold">Services professionnels abordables</p>
            </div>
            <div className="bg-gradient-to-br from-blue-300 to-blue-600 p-10 rounded-3xl shadow-2xl text-white border-4 border-white">
              <div className="text-7xl mb-6">🎯</div>
              <h3 className="font-black text-4xl mb-4">Compétences Variées</h3>
              <p className="text-2xl font-semibold">Analyse, design, communication</p>
            </div>
            <div className="bg-gradient-to-br from-purple-300 to-purple-600 p-10 rounded-3xl shadow-2xl text-white border-4 border-white">
              <div className="text-7xl mb-6">🔄</div>
              <h3 className="font-black text-4xl mb-4">Agence Flexible</h3>
              <p className="text-2xl font-semibold">Adaptation rapide</p>
            </div>
            <div className="bg-gradient-to-br from-orange-300 to-red-600 p-10 rounded-3xl shadow-2xl text-white border-4 border-white">
              <div className="text-7xl mb-6">⚡</div>
              <h3 className="font-black text-4xl mb-4">Réactive</h3>
              <p className="text-2xl font-semibold">Résultats mesurables</p>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-yellow-400 via-orange-500 to-red-500 p-16">
          <h1 className="text-6xl font-black mb-10 text-white drop-shadow-lg text-center">Points Forts</h1>
          <div className="grid grid-cols-3 gap-8">
            <div className="bg-white p-10 rounded-3xl shadow-2xl text-center border-4 border-yellow-300">
              <div className="w-24 h-24 bg-gradient-to-br from-blue-400 to-blue-600 rounded-full flex items-center justify-center mx-auto mb-6 shadow-xl">
                <Users className="w-12 h-12 text-white" />
              </div>
              <h3 className="font-black text-2xl mb-3 text-blue-700">Équipe Pluridisciplinaire</h3>
            </div>
            <div className="bg-white p-10 rounded-3xl shadow-2xl text-center border-4 border-green-300">
              <div className="w-24 h-24 bg-gradient-to-br from-green-400 to-emerald-600 rounded-full flex items-center justify-center mx-auto mb-6 shadow-xl">
                <CheckCircle className="w-12 h-12 text-white" />
              </div>
              <h3 className="font-black text-2xl mb-3 text-green-700">Organisation Claire</h3>
            </div>
            <div className="bg-white p-10 rounded-3xl shadow-2xl text-center border-4 border-purple-300">
              <div className="w-24 h-24 bg-gradient-to-br from-purple-400 to-purple-600 rounded-full flex items-center justify-center mx-auto mb-6 shadow-xl">
                <Target className="w-12 h-12 text-white" />
              </div>
              <h3 className="font-black text-2xl mb-3 text-purple-700">Vision Commune</h3>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'content',
      content: (
        <div className="h-full bg-gradient-to-br from-blue-500 via-indigo-600 to-purple-700 p-16 flex items-center justify-center">
          <div className="max-w-5xl">
            <div className="bg-white/10 backdrop-blur-lg p-20 rounded-3xl shadow-2xl text-white text-center border-8 border-white/30">
              <div className="w-40 h-40 bg-gradient-to-br from-yellow-300 to-orange-400 rounded-full flex items-center justify-center mx-auto mb-10 shadow-2xl border-4 border-white">
                <Award className="w-20 h-20 text-white" />
              </div>
              <h2 className="text-6xl font-black mb-8 drop-shadow-lg">Notre Engagement</h2>
              <p className="text-3xl leading-relaxed font-bold mb-12">
                Transformer notre projet en succès concret
              </p>
            </div>
          </div>
        </div>
      )
    },
    {
      type: 'title',
      content: (
        <div className="flex flex-col items-center justify-center h-full bg-gradient-to-br from-indigo-600 via-purple-600 to-pink-600 text-white">
          <div className="text-center space-y-8">
            <div className="text-8xl mb-8">🚀</div>
            <h1 className="text-7xl font-bold mb-6">Merci !</h1>
            <p className="text-3xl font-light max-w-3xl mx-auto leading-relaxed">
              Prêts à transformer notre projet en succès
            </p>
            <div className="mt-12 space-y-4">
              <p className="text-2xl font-semibold">MEDIA 311 PRO</p>
              <p className="text-xl opacity-90">LET'S GROW TOGETHER</p>
            </div>
          </div>
        </div>
      )
    }
  ];

  const nextSlide = () => {
    setCurrentSlide((prev) => (prev + 1) % slides.length);
  };

  const prevSlide = () => {
    setCurrentSlide((prev) => (prev - 1 + slides.length) % slides.length);
  };

  return (
    <div className="w-full h-screen bg-gray-100 flex flex-col">
      <div className="flex-1 relative overflow-hidden bg-white shadow-2xl">
        {slides[currentSlide].content}
      </div>

      <div className="bg-gray-800 text-white p-6 flex items-center justify-between">
        <button
          onClick={prevSlide}
          className="flex items-center space-x-2 bg-blue-600 hover:bg-blue-700 px-6 py-3 rounded-lg transition-colors disabled:opacity-50"
          disabled={currentSlide === 0}
        >
          <ChevronLeft className="w-5 h-5" />
          <span className="font-semibold">Précédent</span>
        </button>

        <div className="flex items-center space-x-6">
          <span className="text-lg font-semibold">
            Slide {currentSlide + 1} / {slides.length}
          </span>
          <div className="flex space-x-2">
            {slides.map((_, index) => (
              <button
                key={index}
                onClick={() => setCurrentSlide(index)}
                className={`w-3 h-3 rounded-full transition-all ${
                  index === currentSlide
                    ? 'bg-blue-500 w-8'
                    : 'bg-gray-500 hover:bg-gray-400'
                }`}
              />
            ))}
          </div>
        </div>

        <button
          onClick={nextSlide}
          className="flex items-center space-x-2 bg-blue-600 hover:bg-blue-700 px-6 py-3 rounded-lg transition-colors disabled:opacity-50"
          disabled={currentSlide === slides.length - 1}
        >
          <span className="font-semibold">Suivant</span>
          <ChevronRight className="w-5 h-5" />
        </button>
      </div>
    </div>
  );
};

export default Presentation;
