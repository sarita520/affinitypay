[App.tsx](https://github.com/user-attachments/files/23997740/App.tsx)
import React, { useState, useEffect } from 'react';
import { Landing } from './pages/Landing';

// Mock simples do Dashboard para o código não quebrar se faltarem arquivos
const DashboardMock = ({ onBack }) => (
  <div className="min-h-screen bg-slate-900 text-white flex items-center justify-center flex-col p-4">
    <h1 className="text-3xl font-bold mb-4">Painel Administrativo SRT-BANK</h1>
    <p className="mb-8 text-slate-400">Backoffice da AffinityPay e Sistema Bancário.</p>
    <button onClick={onBack} className="bg-blue-600 px-6 py-2 rounded font-bold">Voltar para o Site</button>
  </div>
);

export default function App() {
  const [view, setView] = useState('landing');

  return (
    <>
      {view === 'landing' ? (
        <Landing onLogin={() => setView('dashboard')} theme="dark" toggleTheme={() => {}} />
      ) : (
        <DashboardMock onBack={() => setView('landing')} />
      )}
    </>
  );
}
