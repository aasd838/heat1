import React, { useState, useEffect } from 'react';
import { 
  BookOpen, Calculator, Thermometer, Activity, HelpCircle, 
  Award, Search, Flame, Layers, Zap, TrendingUp, RefreshCw, 
  CheckCircle2, XCircle, Info, ChevronRight, ChevronDown, Play, 
  ArrowRight, Shield, Cpu, Gauge
} from 'lucide-react';

export default function App() {
  const [activeTab, setActiveTab] = useState('curriculum');
  const [selectedLecture, setSelectedLecture] = useState(1);
  const [simType, setSimType] = useState('fin');

  // --- Lecture Data Structure ---
  const lectures = [
    {
      id: 1,
      title: 'Lecture 1: Mechanisms of Heat Transfer',
      arabicTitle: 'آليات انتقال الحرارة',
      summary: 'مقدمة في التوصيل، الحمل، والإشعاع الحراري، وقوانين الطاقة الأساسية.',
      keyConcepts: [
        { name: 'Conduction (التوصيل)', eq: "q'' = -k \\frac{dT}{dx}", desc: "Fourier's Law of Heat Conduction" },
        { name: 'Convection (الحمل)', eq: "q'' = h(T_s - T_\\infty)", desc: "Newton's Law of Cooling" },
        { name: 'Radiation (الإشعاع)', eq: "E = \\epsilon \\sigma T_s^4", desc: "Stefan-Boltzmann Law (\\sigma = 5.67 \\times 10^{-8} W/m^2K^4)" }
      ],
      assumptions: ['1D Steady State', 'Constant Properties', 'Uniform Surface Temp'],
      dataBookRef: 'Table A-1: Thermal Conductivities of Common Materials'
    },
    {
      id: 2,
      title: 'Lecture 2: Steady-State 1-D Conduction',
      arabicTitle: 'التوصيل المستقر في بُعد واحد',
      summary: 'جدران مستوية، أسطوانات، كرات، شبكات المقاومة الحرارية، والتوليد الحراري الداخلي.',
      keyConcepts: [
        { name: 'Plane Wall Resistance', eq: 'R_{th,cond} = \\frac{L}{k A}', desc: 'التوليد الحراري في جدار مستوٍ' },
        { name: 'Cylindrical Resistance', eq: 'R_{th,cyl} = \\frac{\\ln(r_2/r_1)}{2\\pi k L}', desc: 'المقاومة الحرارية لأسطوانة مجوفة' },
        { name: 'Heat Generation Wall', eq: 'T(x) = T_s + \\frac{\\dot{q}L^2}{2k}\\left(1 - \\frac{x^2}{L^2}\\right)', desc: 'أقصى درجة حرارة في منتصف الجدار' }
      ],
      assumptions: ['Steady State', '1-D Flow', 'k = constant', 'Uniform \\dot{q}'],
      dataBookRef: 'Conduction Thermal Resistance Formulas'
    },
    {
      id: 3,
      title: 'Lecture 3: Extended Surfaces (Fins)',
      arabicTitle: 'الأسطح الممتدة (الزعانف)',
      summary: 'معادلة الزعنفة، الشروط الحدية للطرف، كفاءة الزعنفة \\(\\eta_f\\) وفاعليتها \\(\\varepsilon_f\\).',
      keyConcepts: [
        { name: 'Fin Parameter (m)', eq: 'm = \\sqrt{\\frac{h P}{k A_c}}', desc: 'مُعامل المعادلة التفاضلية للزعنفة' },
        { name: 'Insulated Tip Profile', eq: '\\frac{\\theta(x)}{\\theta_b} = \\frac{\\cosh(m(L-x))}{\\cosh(mL)}', desc: 'توزيع الحرارة لزعنفة طرفها معزول' },
        { name: 'Fin Efficiency', eq: '\\eta_f = \\frac{\\tanh(mL)}{mL}', desc: 'نسبة الحرارة المنتقلة للحرارة القصوى النظرية' }
      ],
      assumptions: ['1D conduction along fin', 'Constant h and k', 'Negligible radiation'],
      dataBookRef: 'Fin Efficiency Charts & Geometry Formulas'
    },
    {
      id: 4,
      title: 'Lecture 4: Transient Heat Conduction',
      arabicTitle: 'انتقال الحرارة غير المستقر',
      summary: 'طريقة السعة المجمعة (Lumped Capacitance)، رقم بيوت Bi، رقم فوريه Fo، ومخططات هايسلر.',
      keyConcepts: [
        { name: 'Biot Number', eq: 'Bi = \\frac{h L_c}{k} < 0.1', desc: 'شرط صلاحية طريقة السعة المجمعة' },
        { name: 'Lumped Temp Ratio', eq: '\\frac{T(t) - T_\\infty}{T_i - T_\\infty} = \\exp\\left(-\\frac{t}{\\tau}\\right)', desc: 'تغير الحرارة مع الزمن حيث \\(\\tau = \\frac{\\rho V c_p}{h A_s}\\)' },
        { name: 'Fourier Number', eq: 'Fo = \\frac{\\alpha t}{L_c^2}', desc: 'الزمن الحراري المبعد' }
      ],
      assumptions: ['Bi < 0.1 for Lumped', 'Uniform spatial temp', 'Constant fluid props'],
      dataBookRef: 'Heisler & Grober Charts, Table A-2'
    },
    {
      id: 5,
      title: 'Lecture 5: External Flow Convection',
      arabicTitle: 'الحمل القسري الخارجي',
      summary: 'الطبقة الجدارية الهيدروديناميكية والحرارية، أرقام Re, Pr, Nu، الجريان حول الألواح والأسطوانات وحزم الأنابيب.',
      keyConcepts: [
        { name: 'Reynolds Number', eq: 'Re_x = \\frac{\\rho V x}{\\mu} = \\frac{V x}{\\nu}', desc: 'نسبة قوى القصور الذاتي إلى قوى اللزوجة' },
        { name: 'Prandtl Number', eq: 'Pr = \\frac{\\nu}{\\alpha} = \\frac{\\mu c_p}{k}', desc: 'نسبة الانتشارية الزخامية إلى الحرارية' },
        { name: 'Flat Plate Nu', eq: 'Nu_x = 0.332 Re_x^{1/2} Pr^{1/3}', desc: 'جريان صفيحي على لوح مستوٍ' }
      ],
      assumptions: ['Evaluated at Film Temp T_f = (T_s + T_\\infty)/2', 'Constant free-stream velocity'],
      dataBookRef: 'External Flow Correlations & Tube Bank Tables'
    },
    {
      id: 6,
      title: 'Lecture 6: Natural / Free Convection',
      arabicTitle: 'الحمل الحر / الطبيعي',
      summary: 'قوى الطفو، رقم جراشوف Gr، رقم رايلي Ra، الحمل الحر على الألواح الرأسية والأفقية والتجافيف.',
      keyConcepts: [
        { name: 'Grashof Number', eq: 'Gr_L = \\frac{g \\beta (T_s - T_\\infty) L^3}{\\nu^2}', desc: 'نسبة قوى الطفو إلى قوى اللزوجة' },
        { name: 'Rayleigh Number', eq: 'Ra_L = Gr_L \\cdot Pr', desc: 'محدد طبيعة الجريان (صفيحي أم اضطرابي)' },
        { name: 'Vertical Plate Nu', eq: 'Nu = \\left[0.825 + \\frac{0.387 Ra_L^{1/6}}{(1 + (0.492/Pr)^{9/16})^{8/27}}\\right]^2', desc: 'علاقة تشرشل وتشاو للألواح الرأسية' }
      ],
      assumptions: ['Ideal gas \\beta = 1/T_f (K)', 'Quiescent surrounding fluid'],
      dataBookRef: 'Natural Convection Empirical Correlations'
    },
    {
      id: 7,
      title: 'Lecture 7: Internal Forced Convection',
      arabicTitle: 'الحمل القسري الداخلي',
      summary: 'الجريان داخل الأنابيب، طول المدخل الهيدروديناميكي والحراري، التدفق الحراري الثابت مقابل درجة الحرارة الثابتة.',
      keyConcepts: [
        { name: 'Laminar Tube Nu', eq: 'Nu_D = 4.36 \\text{ (q" const)}, 3.66 \\text{ (T_s const)}', desc: 'جريان مكتمل النمو صفيحي' },
        { name: 'Dittus-Boelter', eq: 'Nu_D = 0.023 Re_D^{0.8} Pr^n', desc: 'جريان مضطرب (n=0.4 تسخين, n=0.3 تبريد)' },
        { name: 'Mean Temp Log', eq: 'q = \\dot{m} c_p (T_{m,o} - T_{m,i})', desc: 'موازنة الطاقة الكلية للأنبوب' }
      ],
      assumptions: ['Re_D > 10,000 for Dittus-Boelter', '0.6 < Pr < 160'],
      dataBookRef: 'Moody Chart, Friction factor relations'
    },
    {
      id: 8,
      title: 'Lecture 8: Radiation Heat Transfer',
      arabicTitle: 'انتقال الحرارة بالإشعاع',
      summary: 'إشعاع الجسم الأسود والأجسام الرمادية، معامِلات الرؤية (View Factors)، الدوائر المكافئة للإشعاع، والحواجز الإشعاعية.',
      keyConcepts: [
        { name: 'Stefan-Boltzmann', eq: 'E_b = \\sigma T^4', desc: 'قدرة الانبعاث للجسم الأسود' },
        { name: 'View Factor Recip.', eq: 'A_1 F_{12} = A_2 F_{21}', desc: 'علاقة التبادلية لمعاملات الرؤية' },
        { name: 'Radiosity Net Q', eq: 'q_{12} = \\frac{\\sigma (T_1^4 - T_2^4)}{\\frac{1-\\epsilon_1}{\\epsilon_1 A_1} + \\frac{1}{A_1 F_{12}} + \\frac{1-\\epsilon_2}{\\epsilon_2 A_2}}', desc: 'التبادل الإشعاعي بين سطحين رماديين' }
      ],
      assumptions: ['Diffuse, gray surfaces', 'Opaque media', 'Uniform radiosities'],
      dataBookRef: 'View Factor Charts, Emissivity Tables'
    },
    {
      id: 9,
      title: 'Lecture 9: Heat Exchangers',
      arabicTitle: 'المبادلات الحرارية',
      summary: 'أنواع المبادلات، طريقة فرق درجات الحرارة اللوجاريتمي (LMTD)، طريقة الفاعلية (\\(\\varepsilon\\)-NTU)، ومعامل الاتساخ.',
      keyConcepts: [
        { name: 'LMTD Equation', eq: '\\Delta T_{lm} = \\frac{\\Delta T_1 - \\Delta T_2}{\\ln(\\Delta T_1 / \\Delta T_2)}', desc: 'المتوسط اللوجاريتمي لفرق الحرارة' },
        { name: 'Effectiveness', eq: '\\varepsilon = \\frac{q}{q_{max}} = \\frac{q}{C_{min}(T_{h,in} - T_{c,in})}', desc: 'فاعلية المبادل الحراري' },
        { name: 'NTU Definition', eq: 'NTU = \\frac{U A_s}{C_{min}}', desc: 'عدد وحدات النقل الحراري' }
      ],
      assumptions: ['Steady state', 'Constant overall U', 'No heat loss to surroundings'],
      dataBookRef: 'LMTD Correction Factor Charts, NTU Effectiveness Relations'
    }
  ];

  // --- Fin Simulator State ---
  const [finK, setFinK] = useState(200); // Aluminum W/mK
  const [finH, setFinH] = useState(50);  // W/m2K
  const [finL, setFinL] = useState(0.1);  // 10 cm
  const [finP, setFinP] = useState(0.04); // 4 cm perimeter
  const [finAc, setFinAc] = useState(0.0001); // 1 cm2 area
  const [finTb, setFinTb] = useState(100); // C
  const [finTinf, setFinTinf] = useState(25); // C

  // --- Fin Calculations ---
  const m = Math.sqrt((finH * finP) / (finK * finAc));
  const mL = m * finL;
  const qFinInsulated = Math.sqrt(finH * finP * finK * finAc) * (finTb - finTinf) * Math.tanh(mL);
  const etaFin = Math.tanh(mL) / mL;
  const epsilonFin = qFinInsulated / (finH * finAc * (finTb - finTinf));

  // Temp profile points
  const finPoints = Array.from({ length: 20 }, (_, i) => {
    const x = (i / 19) * finL;
    const thetaX = (finTb - finTinf) * (Math.cosh(m * (finL - x)) / Math.cosh(mL));
    return { x: x.toFixed(3), T: (thetaX + finTinf).toFixed(1) };
  });

  // --- Transient Simulator State ---
  const [trK, setTrK] = useState(50);
  const [trH, setTrH] = useState(100);
  const [trRho, setTrRho] = useState(7800);
  const [trCp, setTrCp] = useState(460);
  const [trLc, setTrLc] = useState(0.01);
  const [trTi, setTrTi] = useState(300);
  const [trTinf, setTrTinf] = useState(25);
  const [trTime, setTrTime] = useState(60);

  const biNum = (trH * trLc) / trK;
  const tau = (trRho * trLc * trCp) / trH;
  const alpha = trK / (trRho * trCp);
  const foNum = (alpha * trTime) / (trLc * trLc);
  const trTempAtT = trTinf + (trTi - trTinf) * Math.exp(-trTime / tau);

  const trPoints = Array.from({ length: 20 }, (_, i) => {
    const t = (i / 19) * (tau * 3);
    const T = trTinf + (trTi - trTinf) * Math.exp(-t / tau);
    return { t: Math.round(t), T: T.toFixed(1) };
  });

  // --- Socratic Tutor State ---
  const [socStep, setSocStep] = useState(1);
  const [socUserChoice, setSocUserChoice] = useState(null);
  const [socFeedback, setSocFeedback] = useState('');

  const handleSocraticChoice = (choiceIndex, isCorrect, feedback) => {
    setSocUserChoice(choiceIndex);
    setSocFeedback(feedback);
  };

  // --- Data Book Air Properties State ---
  const [airTemp, setAirTemp] = useState(300); // Kelvin
  const getAirProperties = (T) => {
    // Linear approximation around 300K - 400K for demo purposes
    const rho = (1.1614 - 0.003 * (T - 300)).toFixed(3);
    const cp = (1007 + 0.1 * (T - 300)).toFixed(0);
    const k = (0.0263 + 0.00007 * (T - 300)).toFixed(4);
    const nu = (15.89 + 0.1 * (T - 300)).toFixed(2);
    const Pr = (0.707 - 0.0001 * (T - 300)).toFixed(3);
    return { rho, cp, k, nu, Pr };
  };
  const airProps = getAirProperties(airTemp);

  // --- Quiz Engine State ---
  const [quizIndex, setQuizIndex] = useState(0);
  const [quizSelectedOption, setQuizSelectedOption] = useState(null);
  const [quizScore, setQuizScore] = useState(0);
  const [quizSubmitted, setQuizSubmitted] = useState(false);

  const quizQuestions = [
    {
      q: 'ما هو الشرط الهندسي الفيزيائي لتطبيق طريقة السعة المجمعة (Lumped Capacitance Method) في انتقال الحرارة غير المستقر؟',
      options: [
        'أن يكون رقم فوريه Fo > 1.0',
        'أن يكون رقم بيوت Bi < 0.1',
        'أن تكون الموصلية الحرارية k صغيرة جداً',
        'أن تكون سرعة المائع V > 10 m/s'
      ],
      correct: 1,
      explanation: 'صحيح! عندما يكون Bi = h L_c / k < 0.1، تكون المقاومة الحرارية بالتوصيل داخل الجسم مهملة مقارنة بالمقاومة بالحمل على السطح، مما يجعل توزيع الحرارة داخل الجسم متجانساً تقريباً.'
    },
    {
      q: 'عند حساب نقل الحرارة بالحمل الحر (Natural Convection) على لوح رأسي، ما هو الرقم المبعد المعبر عن نسبة قوى الطفو إلى قوى اللزوجة؟',
      options: [
        'Reynolds Number (Re)',
        'Prandtl Number (Pr)',
        'Grashof Number (Gr)',
        'Nusselt Number (Nu)'
      ],
      correct: 2,
      explanation: 'ممتاز! رقم جراشوف Gr = g \\beta (T_s - T_\\infty) L^3 / \\nu^2 يقيس التوازن بين قوى الطفو الناتجة عن اختلاف الكثافة وقوى اللزوجة المعيقة للحركة.'
    },
    {
      q: 'زعنفة طويلة جداً (Infinitely Long Fin) ذات مقطع ثابت، ما هي كفاءتها النظرية \\(\\eta_f\\) إذا كان \\(mL = 2.0\\)؟',
      options: [
        '100%',
        '50%',
        '48.2%',
        '33.3%'
      ],
      correct: 2,
      explanation: 'أحسنت! لحساب كفاءة الزعنفة المقفلة أو الطويلة، \\(\\eta_f = \\tanh(mL) / mL\\). بالتعويض: \\(\\tanh(2.0)/2.0 = 0.964 / 2.0 = 0.482\\) أي 48.2%.'
    }
  ];

  const handleQuizAnswer = (optIndex) => {
    if (quizSubmitted) return;
    setQuizSelectedOption(optIndex);
  };

  const submitQuizAnswer = () => {
    if (quizSelectedOption === null) return;
    setQuizSubmitted(true);
    if (quizSelectedOption === quizQuestions[quizIndex].correct) {
      setQuizScore(quizScore + 1);
    }
  };

  const nextQuizQuestion = () => {
    setQuizSelectedOption(null);
    setQuizSubmitted(false);
    if (quizIndex < quizQuestions.length - 1) {
      setQuizIndex(quizIndex + 1);
    } else {
      alert(`أكملت الاختبار! نتيجتك: ${quizScore + (quizSelectedOption === quizQuestions[quizIndex].correct ? 1 : 0)} من ${quizQuestions.length}`);
      setQuizIndex(0);
      setQuizScore(0);
    }
  };

  return (
    <div className="min-h-screen bg-slate-950 text-slate-100 font-sans dir-rtl" dir="rtl">
      
      {/* Header Banner */}
      <header className="border-b border-slate-800 bg-slate-900/80 backdrop-blur sticky top-0 z-50">
        <div className="max-w-7xl mx-auto px-4 py-3 flex flex-wrap justify-between items-center gap-4">
          <div className="flex items-center space-x-3 space-x-reverse">
            <div className="bg-gradient-to-tr from-amber-500 to-orange-600 p-2.5 rounded-xl text-slate-950 shadow-lg shadow-orange-500/20">
              <Flame size={28} className="animate-pulse" />
            </div>
            <div>
              <h1 className="text-xl font-bold bg-gradient-to-r from-amber-400 via-orange-300 to-amber-200 bg-clip-text text-transparent">
                مستكشف انتقال الحرارة | Heat Transfer Explorer
              </h1>
              <p className="text-xs text-slate-400">المنصة الهندسية التفاعلية للمنهج الجامعي وسجل البيانات (Data Book)</p>
            </div>
          </div>

          {/* Navigation Tabs */}
          <nav className="flex items-center gap-1 bg-slate-800/80 p-1 rounded-xl border border-slate-700/60 overflow-x-auto max-w-full">
            <button
              onClick={() => setActiveTab('curriculum')}
              className={`flex items-center gap-2 px-3.5 py-1.5 rounded-lg text-xs font-medium transition-all ${
                activeTab === 'curriculum'
                  ? 'bg-orange-500 text-slate-950 shadow-md font-semibold'
                  : 'text-slate-300 hover:bg-slate-700/50'
              }`}
            >
              <BookOpen size={15} />
              المنهج الدراسي (Lectures)
            </button>
            <button
              onClick={() => setActiveTab('simulators')}
              className={`flex items-center gap-2 px-3.5 py-1.5 rounded-lg text-xs font-medium transition-all ${
                activeTab === 'simulators'
                  ? 'bg-orange-500 text-slate-950 shadow-md font-semibold'
                  : 'text-slate-300 hover:bg-slate-700/50'
              }`}
            >
              <Activity size={15} />
              المحاكيات التفاعلية
            </button>
            <button
              onClick={() => setActiveTab('databook')}
              className={`flex items-center gap-2 px-3.5 py-1.5 rounded-lg text-xs font-medium transition-all ${
                activeTab === 'databook'
                  ? 'bg-orange-500 text-slate-950 shadow-md font-semibold'
                  : 'text-slate-300 hover:bg-slate-700/50'
              }`}
            >
              <Layers size={15} />
              سجل البيانات (Data Book)
            </button>
            <button
              onClick={() => setActiveTab('socratic')}
              className={`flex items-center gap-2 px-3.5 py-1.5 rounded-lg text-xs font-medium transition-all ${
                activeTab === 'socratic'
                  ? 'bg-orange-500 text-slate-950 shadow-md font-semibold'
                  : 'text-slate-300 hover:bg-slate-700/50'
              }`}
            >
              <HelpCircle size={15} />
              المعلم السقراطي
            </button>
            <button
              onClick={() => setActiveTab('quiz')}
              className={`flex items-center gap-2 px-3.5 py-1.5 rounded-lg text-xs font-medium transition-all ${
                activeTab === 'quiz'
                  ? 'bg-orange-500 text-slate-950 shadow-md font-semibold'
                  : 'text-slate-300 hover:bg-slate-700/50'
              }`}
            >
              <Award size={15} />
              مختبر الاختبارات
            </button>
          </nav>
        </div>
      </header>

      {/* Main Content Area */}
      <main className="max-w-7xl mx-auto px-4 py-6">

        {/* ================= TAB 1: CURRICULUM OVERVIEW ================= */}
        {activeTab === 'curriculum' && (
          <div className="grid grid-cols-1 lg:grid-cols-12 gap-6">
            
            {/* Lecture Selection Sidebar */}
            <div className="lg:col-span-4 bg-slate-900 border border-slate-800 rounded-2xl p-4 shadow-xl">
              <h2 className="text-sm font-bold text-slate-300 mb-3 flex items-center gap-2 border-b border-slate-800 pb-2">
                <BookOpen size={18} className="text-orange-400" />
                محاضرات المنهج (Lectures 1 - 9)
              </h2>
              <div className="space-y-2 max-h-[600px] overflow-y-auto pr-1">
                {lectures.map((lect) => (
                  <button
                    key={lect.id}
                    onClick={() => setSelectedLecture(lect.id)}
                    className={`w-full text-right p-3 rounded-xl border transition-all flex flex-col gap-1 ${
                      selectedLecture === lect.id
                        ? 'bg-orange-500/10 border-orange-500/50 text-orange-200'
                        : 'bg-slate-800/40 border-slate-800 text-slate-400 hover:border-slate-700 hover:text-slate-200'
                    }`}
                  >
                    <div className="flex justify-between items-center">
                      <span className="text-xs font-bold text-orange-400">Lecture {lect.id}</span>
                      <span className="text-[10px] bg-slate-800 px-2 py-0.5 rounded text-slate-400">
                        {lect.assumptions.length} الفروض الرئيسية
                      </span>
                    </div>
                    <div className="text-sm font-semibold text-slate-100">{lect.arabicTitle}</div>
                    <div className="text-xs text-slate-400 line-clamp-1">{lect.title}</div>
                  </button>
                ))}
              </div>
            </div>

            {/* Selected Lecture Detailed View */}
            <div className="lg:col-span-8 space-y-6">
              {(() => {
                const current = lectures.find((l) => l.id === selectedLecture);
                return (
                  <div className="bg-slate-900 border border-slate-800 rounded-2xl p-6 shadow-xl space-y-6">
                    <div className="border-b border-slate-800 pb-4">
                      <span className="text-xs font-bold text-orange-400 bg-orange-500/10 border border-orange-500/20 px-3 py-1 rounded-full">
                        {current.title}
                      </span>
                      <h2 className="text-2xl font-bold text-slate-100 mt-2">{current.arabicTitle}</h2>
                      <p className="text-sm text-slate-400 mt-1">{current.summary}</p>
                    </div>

                    {/* Key Concepts & Equations */}
                    <div>
                      <h3 className="text-md font-bold text-slate-200 mb-3 flex items-center gap-2">
                        <Zap size={18} className="text-amber-400" />
                        المفاهيم والمعادلات الحاكمة (Governing Equations)
                      </h3>
                      <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
                        {current.keyConcepts.map((concept, idx) => (
                          <div key={idx} className="bg-slate-950 border border-slate-800 p-4 rounded-xl space-y-2">
                            <div className="text-xs font-bold text-orange-300">{concept.name}</div>
                            <div className="bg-slate-900 p-2.5 rounded-lg font-mono text-xs text-emerald-400 text-center dir-ltr border border-slate-800">
                              {concept.eq}
                            </div>
                            <div className="text-xs text-slate-400">{concept.desc}</div>
                          </div>
                        ))}
                      </div>
                    </div>

                    {/* Engineering Assumptions & Data Book Cross Reference */}
                    <div className="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
                      <div className="bg-slate-950/60 border border-slate-800/80 p-4 rounded-xl space-y-2">
                        <h4 className="text-xs font-bold text-slate-300 flex items-center gap-1.5">
                          <CheckCircle2 size={15} className="text-emerald-400" />
                          الافتراضات الهندسية الشائعة (Assumptions)
                        </h4>
                        <ul className="text-xs text-slate-400 space-y-1 list-disc list-inside">
                          {current.assumptions.map((asm, i) => (
                            <li key={i}>{asm}</li>
                          ))}
                        </ul>
                      </div>

                      <div className="bg-slate-950/60 border border-slate-800/80 p-4 rounded-xl space-y-2">
                        <h4 className="text-xs font-bold text-slate-300 flex items-center gap-1.5">
                          <Layers size={15} className="text-sky-400" />
                          مرجع جدول البيانات (Data Book Ref)
                        </h4>
                        <p className="text-xs text-sky-300 font-mono bg-sky-950/40 p-2 rounded border border-sky-900/50">
                          {current.dataBookRef}
                        </p>
                      </div>
                    </div>

                  </div>
                );
              })()}
            </div>

          </div>
        )}

        {/* ================= TAB 2: INTERACTIVE SIMULATORS ================= */}
        {activeTab === 'simulators' && (
          <div className="space-y-6">
            
            {/* Simulator Type Switcher */}
            <div className="flex gap-2 border-b border-slate-800 pb-3">
              <button
                onClick={() => setSimType('fin')}
                className={`px-4 py-2 rounded-xl text-xs font-bold transition-all ${
                  simType === 'fin'
                    ? 'bg-orange-500 text-slate-950'
                    : 'bg-slate-900 text-slate-400 hover:text-slate-200'
                }`}
              >
                محاكاة الزعنفة الحرارية (Fin Analysis - Lecture 3)
              </button>
              <button
                onClick={() => setSimType('transient')}
                className={`px-4 py-2 rounded-xl text-xs font-bold transition-all ${
                  simType === 'transient'
                    ? 'bg-orange-500 text-slate-950'
                    : 'bg-slate-900 text-slate-400 hover:text-slate-200'
                }`}
              >
                الحرارة غير المستقرة والسعة المجمعة (Transient Conduction - Lecture 4)
              </button>
            </div>

            {/* SIMULATOR 1: FIN HEAT TRANSFER */}
            {simType === 'fin' && (
              <div className="grid grid-cols-1 lg:grid-cols-12 gap-6">
                
                {/* Inputs Column */}
                <div className="lg:col-span-5 bg-slate-900 border border-slate-800 p-5 rounded-2xl space-y-4 shadow-xl">
                  <h3 className="text-sm font-bold text-orange-400 border-b border-slate-800 pb-2 flex items-center gap-2">
                    <Gauge size={18} />
                    مدخلات محاكاة الزعنفة (Fin Inputs)
                  </h3>

                  <div className="space-y-3 text-xs">
                    <div>
                      <div className="flex justify-between text-slate-300 mb-1">
                        <span>الموصلية الحرارية للزعنفة \\(k\\) [W/m·K]:</span>
                        <span className="font-mono text-orange-400">{finK}</span>
                      </div>
                      <input
                        type="range"
                        min="10"
                        max="400"
                        value={finK}
                        onChange={(e) => setFinK(Number(e.target.value))}
                        className="w-full accent-orange-500"
                      />
                    </div>

                    <div>
                      <div className="flex justify-between text-slate-300 mb-1">
                        <span>معامل الحمل الحراري \\(h\\) [W/m²·K]:</span>
                        <span className="font-mono text-orange-400">{finH}</span>
                      </div>
                      <input
                        type="range"
                        min="5"
                        max="200"
                        value={finH}
                        onChange={(e) => setFinH(Number(e.target.value))}
                        className="w-full accent-orange-500"
                      />
                    </div>

                    <div>
                      <div className="flex justify-between text-slate-300 mb-1">
                        <span>طول الزعنفة \\(L\\) [m]:</span>
                        <span className="font-mono text-orange-400">{finL}</span>
                      </div>
                      <input
                        type="range"
                        min="0.02"
                        max="0.5"
                        step="0.01"
                        value={finL}
                        onChange={(e) => setFinL(Number(e.target.value))}
                        className="w-full accent-orange-500"
                      />
                    </div>

                    <div className="grid grid-cols-2 gap-3 pt-2 border-t border-slate-800">
                      <div>
                        <label className="block text-slate-400 mb-1">درجة حرارة القاعدة \\(T_b\\) (°C):</label>
                        <input
                          type="number"
                          value={finTb}
                          onChange={(e) => setFinTb(Number(e.target.value))}
                          className="w-full bg-slate-950 border border-slate-800 rounded p-1.5 font-mono text-orange-300"
                        />
                      </div>
                      <div>
                        <label className="block text-slate-400 mb-1">حرارة المائع المحيط \\(T_\\infty\\) (°C):</label>
                        <input
                          type="number"
                          value={finTinf}
                          onChange={(e) => setFinTinf(Number(e.target.value))}
                          className="w-full bg-slate-950 border border-slate-800 rounded p-1.5 font-mono text-orange-300"
                        />
                      </div>
                    </div>
                  </div>

                  {/* Calculated Results Box */}
                  <div className="bg-slate-950 border border-slate-800 p-4 rounded-xl space-y-2 text-xs">
                    <div className="font-bold text-slate-200 border-b border-slate-800 pb-1">النتائج المحسوبة:</div>
                    <div className="flex justify-between">
                      <span className="text-slate-400">معامل الزعنفة \\(m\\):</span>
                      <span className="font-mono text-emerald-400">{m.toFixed(2)} m⁻¹</span>
                    </div>
                    <div className="flex justify-between">
                      <span className="text-slate-400">المقدار \\(m L\\):</span>
                      <span className="font-mono text-emerald-400">{mL.toFixed(3)}</span>
                    </div>
                    <div className="flex justify-between">
                      <span className="text-slate-400">معدل نقل الحرارة \\(q_f\\):</span>
                      <span className="font-mono text-amber-400">{qFinInsulated.toFixed(2)} W</span>
                    </div>
                    <div className="flex justify-between">
                      <span className="text-slate-400">كفاءة الزعنفة \\(\\eta_f\\):</span>
                      <span className="font-mono text-sky-400">{(etaFin * 100).toFixed(1)}%</span>
                    </div>
                    <div className="flex justify-between">
                      <span className="text-slate-400">فاعلية الزعنفة \\(\\varepsilon_f\\):</span>
                      <span className="font-mono text-indigo-400">{epsilonFin.toFixed(2)}</span>
                    </div>
                  </div>
                </div>

                {/* Plot Column */}
                <div className="lg:col-span-7 bg-slate-900 border border-slate-800 p-5 rounded-2xl space-y-4 shadow-xl">
                  <h3 className="text-sm font-bold text-slate-200 flex items-center justify-between">
                    <span>مخطط توزيع الحرارة على طول الزعنفة \\(T(x)\\)</span>
                    <span className="text-xs text-slate-400 font-normal">الحالة: طرف معزول (Insulated Tip)</span>
                  </h3>

                  {/* SVG Line Chart */}
                  <div className="bg-slate-950 border border-slate-800 p-4 rounded-xl h-64 flex flex-col justify-between relative">
                    <svg className="w-full h-48 overflow-visible">
                      {/* Grid lines */}
                      <line x1="0" y1="0" x2="100%" y2="0" stroke="#334155" strokeDasharray="4" />
                      <line x1="0" y1="50%" x2="100%" y2="50%" stroke="#334155" strokeDasharray="4" />
                      <line x1="0" y1="100%" x2="100%" y2="100%" stroke="#334155" />

                      {/* Temperature Curve */}
                      <path
                        d={finPoints.reduce((acc, point, idx) => {
                          const xPct = (idx / (finPoints.length - 1)) * 100;
                          // Scale T between Tinf and Tb
                          const tNum = parseFloat(point.T);
                          const yPct = 100 - ((tNum - finTinf) / (finTb - finTinf)) * 100;
                          return `${acc} ${idx === 0 ? 'M' : 'L'} ${xPct}% ${yPct}%`;
                        }, '')}
                        fill="none"
                        stroke="#f97316"
                        strokeWidth="3"
                      />
                    </svg>

                    <div className="flex justify-between text-[10px] text-slate-500 pt-2 border-t border-slate-800">
                      <span>القاعدة x = 0 (T = {finTb}°C)</span>
                      <span>طول الزعنفة x = {finL}m</span>
                      <span>الطرف x = L (T = {finPoints[finPoints.length - 1].T}°C)</span>
                    </div>
                  </div>

                  <div className="bg-slate-950/40 p-3 rounded-xl border border-slate-800 text-xs text-slate-400">
                    <span className="text-orange-400 font-bold">توجيه أستاذ المادة:</span> لاحظ أنه كلما زادت قيمة الموصلية الحرارية \\(k\\)، يقل الانحدار الحراري ويصبح الطرف أكثر سخونة، مما يرفع من كفاءة الزعنفة \\(\\eta_f\\).
                  </div>
                </div>

              </div>
            )}

            {/* SIMULATOR 2: TRANSIENT HEAT CONDUCTION */}
            {simType === 'transient' && (
              <div className="grid grid-cols-1 lg:grid-cols-12 gap-6">
                
                {/* Inputs Column */}
                <div className="lg:col-span-5 bg-slate-900 border border-slate-800 p-5 rounded-2xl space-y-4 shadow-xl">
                  <h3 className="text-sm font-bold text-orange-400 border-b border-slate-800 pb-2 flex items-center gap-2">
                    <Thermometer size={18} />
                    مدخلات السعة المجمعة (Lumped System Inputs)
                  </h3>

                  <div className="space-y-3 text-xs">
                    <div>
                      <div className="flex justify-between text-slate-300 mb-1">
                        <span>معامل الحمل الحراري \\(h\\) [W/m²·K]:</span>
                        <span className="font-mono text-orange-400">{trH}</span>
                      </div>
                      <input
                        type="range"
                        min="10"
                        max="500"
                        value={trH}
                        onChange={(e) => setTrH(Number(e.target.value))}
                        className="w-full accent-orange-500"
                      />
                    </div>

                    <div>
                      <div className="flex justify-between text-slate-300 mb-1">
                        <span>الطول المميز \\(L_c = V/A_s\\) [m]:</span>
                        <span className="font-mono text-orange-400">{trLc}</span>
                      </div>
                      <input
                        type="range"
                        min="0.001"
                        max="0.05"
                        step="0.001"
                        value={trLc}
                        onChange={(e) => setTrLc(Number(e.target.value))}
                        className="w-full accent-orange-500"
                      />
                    </div>

                    <div>
                      <div className="flex justify-between text-slate-300 mb-1">
                        <span>الزمن المستغرق \\(t\\) [seconds]:</span>
                        <span className="font-mono text-orange-400">{trTime} s</span>
                      </div>
                      <input
                        type="range"
                        min="1"
                        max="300"
                        value={trTime}
                        onChange={(e) => setTrTime(Number(e.target.value))}
                        className="w-full accent-orange-500"
                      />
                    </div>
                  </div>

                  {/* Biot Number Check Box */}
                  <div className="bg-slate-950 border border-slate-800 p-4 rounded-xl space-y-2 text-xs">
                    <div className="font-bold text-slate-200 border-b border-slate-800 pb-1">تحليل رقم بيوت (Biot Number Check):</div>
                    <div className="flex justify-between">
                      <span className="text-slate-400">رقم بيوت \\(Bi = h L_c / k\\):</span>
                      <span className={`font-mono font-bold ${biNum < 0.1 ? 'text-emerald-400' : 'text-rose-400'}`}>
                        {biNum.toFixed(4)}
                      </span>
                    </div>
                    <div className="text-[11px] p-2 rounded bg-slate-900 border border-slate-800">
                      {biNum < 0.1 ? (
                        <span className="text-emerald-400 font-semibold">
                          ✓ الشرط متوفر (Bi &lt; 0.1): طريقة السعة المجمعة دقيقة ومقبولة!
                        </span>
                      ) : (
                        <span className="text-rose-400 font-semibold">
                          ✕ الشرط غير متوفر (Bi &gt; 0.1): يوجد تدرج حراري داخلي، يلزم استخدام مخططات هايسلر (Heisler Charts).
                        </span>
                      )}
                    </div>
                    <div className="flex justify-between pt-1">
                      <span className="text-slate-400">الثابت الزمني \\(\\tau\\):</span>
                      <span className="font-mono text-amber-400">{tau.toFixed(1)} seconds</span>
                    </div>
                    <div className="flex justify-between">
                      <span className="text-slate-400">الحرارة عند الزمن t:</span>
                      <span className="font-mono text-sky-400">{trTempAtT.toFixed(1)} °C</span>
                    </div>
                  </div>

                </div>

                {/* Plot Column */}
                <div className="lg:col-span-7 bg-slate-900 border border-slate-800 p-5 rounded-2xl space-y-4 shadow-xl">
                  <h3 className="text-sm font-bold text-slate-200">
                    منحنى التبريد الزمني exponential decay curve \\(T(t)\\)
                  </h3>

                  <div className="bg-slate-950 border border-slate-800 p-4 rounded-xl h-64 flex flex-col justify-between">
                    <svg className="w-full h-48 overflow-visible">
                      <line x1="0" y1="0" x2="100%" y2="0" stroke="#334155" strokeDasharray="4" />
                      <line x1="0" y1="100%" x2="100%" y2="100%" stroke="#334155" />

                      <path
                        d={trPoints.reduce((acc, point, idx) => {
                          const xPct = (idx / (trPoints.length - 1)) * 100;
                          const tNum = parseFloat(point.T);
                          const yPct = 100 - ((tNum - trTinf) / (trTi - trTinf)) * 100;
                          return `${acc} ${idx === 0 ? 'M' : 'L'} ${xPct}% ${yPct}%`;
                        }, '')}
                        fill="none"
                        stroke="#38bdf8"
                        strokeWidth="3"
                      />
                    </svg>

                    <div className="flex justify-between text-[10px] text-slate-500 pt-2 border-t border-slate-800">
                      <span>الزمن t = 0 (T = {trTi}°C)</span>
                      <span>t = {trTime}s (T = {trTempAtT.toFixed(1)}°C)</span>
                      <span>الاستقرار t → ∞ (T = {trTinf}°C)</span>
                    </div>
                  </div>
                </div>

              </div>
            )}

          </div>
        )}

        {/* ================= TAB 3: DATA BOOK LOOKUP ================= */}
        {activeTab === 'databook' && (
          <div className="space-y-6">
            <div className="bg-slate-900 border border-slate-800 rounded-2xl p-6 shadow-xl space-y-6">
              
              <div className="flex justify-between items-center border-b border-slate-800 pb-4">
                <div>
                  <h2 className="text-lg font-bold text-slate-100 flex items-center gap-2">
                    <Layers className="text-orange-400" size={22} />
                    سجل البيانات الهندسية (Interactive Data Book)
                  </h2>
                  <p className="text-xs text-slate-400">خواص الهواء والماء وتقييم الخواص عند درجة حرارة الفيلم (Film Temperature \\(T_f\\))</p>
                </div>
              </div>

              {/* Air Thermophysical Properties Calculator */}
              <div className="bg-slate-950 border border-slate-800 p-5 rounded-xl space-y-4">
                <h3 className="text-sm font-bold text-orange-300">
                  خواص الهواء الجاف عند الضغط الجوي (Air Properties at 1 atm)
                </h3>

                <div className="flex items-center gap-4 text-xs">
                  <label className="text-slate-300">درجة حرارة الفيلم \\(T_f\\) (Kelvin):</label>
                  <input
                    type="range"
                    min="250"
                    max="500"
                    value={airTemp}
                    onChange={(e) => setAirTemp(Number(e.target.value))}
                    className="w-48 accent-orange-500"
                  />
                  <span className="font-mono text-orange-400 font-bold">{airTemp} K ({airTemp - 273}°C)</span>
                </div>

                <div className="grid grid-cols-2 md:grid-cols-5 gap-3 pt-2">
                  <div className="bg-slate-900 p-3 rounded-lg border border-slate-800 text-center">
                    <div className="text-[10px] text-slate-400">الكثافة \\(\\rho\\)</div>
                    <div className="text-sm font-mono text-emerald-400 font-bold">{airProps.rho}</div>
                    <div className="text-[9px] text-slate-500">kg/m³</div>
                  </div>
                  <div className="bg-slate-900 p-3 rounded-lg border border-slate-800 text-center">
                    <div className="text-[10px] text-slate-400">الحرارة النوعية \\(c_p\\)</div>
                    <div className="text-sm font-mono text-emerald-400 font-bold">{airProps.cp}</div>
                    <div className="text-[9px] text-slate-500">J/kg·K</div>
                  </div>
                  <div className="bg-slate-900 p-3 rounded-lg border border-slate-800 text-center">
                    <div className="text-[10px] text-slate-400">الموصلية \\(k\\)</div>
                    <div className="text-sm font-mono text-emerald-400 font-bold">{airProps.k}</div>
                    <div className="text-[9px] text-slate-500">W/m·K</div>
                  </div>
                  <div className="bg-slate-900 p-3 rounded-lg border border-slate-800 text-center">
                    <div className="text-[10px] text-slate-400">اللزوجة الحركية \\(\\nu\\)</div>
                    <div className="text-sm font-mono text-emerald-400 font-bold">{airProps.nu} ×10⁻⁶</div>
                    <div className="text-[9px] text-slate-500">m²/s</div>
                  </div>
                  <div className="bg-slate-900 p-3 rounded-lg border border-slate-800 text-center">
                    <div className="text-[10px] text-slate-400">رقم برانتل \\(Pr\\)</div>
                    <div className="text-sm font-mono text-amber-400 font-bold">{airProps.Pr}</div>
                    <div className="text-[9px] text-slate-500">Dimensionless</div>
                  </div>
                </div>
              </div>

            </div>
          </div>
        )}

        {/* ================= TAB 4: SOCRATIC TUTOR ================= */}
        {activeTab === 'socratic' && (
          <div className="bg-slate-900 border border-slate-800 rounded-2xl p-6 shadow-xl space-y-6">
            <div className="border-b border-slate-800 pb-4">
              <span className="text-xs font-bold text-emerald-400 bg-emerald-500/10 px-3 py-1 rounded-full border border-emerald-500/20">
                طريقة التفكير الهندسي السقراطي (Socratic Method)
              </span>
              <h2 className="text-xl font-bold text-slate-100 mt-2">مسألة تفاعلية موجهة: تصميم المبرد الحراري لرقاقة إلكترونية</h2>
              <p className="text-xs text-slate-400">سيقوم المعلم بطرح أسئلة متدرجة لتصل بنفسك إلى الحل الصحيح دون إعطاء إجابات جاهزة.</p>
            </div>

            {/* Step 1 */}
            {socStep === 1 && (
              <div className="bg-slate-950 border border-slate-800 p-5 rounded-xl space-y-4">
                <div className="text-xs text-orange-400 font-bold">الخطوة 1: تحديد آليات نقل الحرارة الحاكمة</div>
                <p className="text-sm text-slate-200">
                  لدينا رقاقة إلكترونية تُولد حرارة بقدرة 15 واط، ويتصل بها مبرد ألومنيوم (Heat Sink) مزود بزعانف ومحاط بهواء متحرك بوساطة مروحة. ما هي آليات نقل الحرارة التراكمية في هذا النظام؟
                </p>

                <div className="space-y-2 text-xs">
                  {[
                    { text: 'توصيل داخل الرقاقة والزعنفة + حمل حراري قسري مع الهواء', correct: true, fb: 'إجابة ممتازة! التوصيل ينقل الحرارة عبر معدن الزعنفة، والحمل القسري ينقلها للهواء المتحرك بفعل المروحة.' },
                    { text: 'إشعاع حراري فقط', correct: false, fb: 'تذكر أن وجود مروحة يجعل الحمل القسري هو الآلية السائدة لنقل الحرارة.' },
                    { text: 'حمل حر طبيعي فقط', correct: false, fb: 'وجود المروحة يحول الحمل من حر (Natural) إلى قسري (Forced).' }
                  ].map((opt, idx) => (
                    <button
                      key={idx}
                      onClick={() => handleSocraticChoice(idx, opt.correct, opt.fb)}
                      className={`w-full text-right p-3 rounded-lg border transition-all ${
                        socUserChoice === idx
                          ? opt.correct
                            ? 'bg-emerald-500/10 border-emerald-500 text-emerald-300'
                            : 'bg-rose-500/10 border-rose-500 text-rose-300'
                          : 'bg-slate-900 border-slate-800 text-slate-300 hover:border-slate-700'
                      }`}
                    >
                      {opt.text}
                    </button>
                  ))}
                </div>

                {socFeedback && (
                  <div className="p-3 bg-slate-900 rounded-lg border border-slate-800 text-xs text-slate-300">
                    {socFeedback}
                  </div>
                )}
              </div>
            )}
          </div>
        )}

        {/* ================= TAB 5: QUIZ ENGINE ================= */}
        {activeTab === 'quiz' && (
          <div className="bg-slate-900 border border-slate-800 rounded-2xl p-6 shadow-xl space-y-6">
            <div className="flex justify-between items-center border-b border-slate-800 pb-4">
              <div>
                <h2 className="text-lg font-bold text-slate-100">مختبر تقييم المفاهيم الهندسية (Quiz Laboratory)</h2>
                <p className="text-xs text-slate-400">اختبر فهمك الأكاديمي لمواضيع المنهج من المحاضرة 1 إلى 9</p>
              </div>
              <div className="text-xs font-mono bg-slate-800 px-3 py-1.5 rounded-lg text-orange-400">
                السؤال {quizIndex + 1} من {quizQuestions.length}
              </div>
            </div>

            {/* Question Card */}
            <div className="bg-slate-950 border border-slate-800 p-5 rounded-xl space-y-4">
              <h3 className="text-sm font-bold text-slate-200">{quizQuestions[quizIndex].q}</h3>

              <div className="space-y-2 text-xs">
                {quizQuestions[quizIndex].options.map((opt, idx) => (
                  <button
                    key={idx}
                    onClick={() => handleQuizAnswer(idx)}
                    className={`w-full text-right p-3 rounded-lg border transition-all ${
                      quizSelectedOption === idx
                        ? 'bg-orange-500/20 border-orange-500 text-orange-200 font-bold'
                        : 'bg-slate-900 border-slate-800 text-slate-300 hover:border-slate-700'
                    }`}
                  >
                    {opt}
                  </button>
                ))}
              </div>

              {!quizSubmitted ? (
                <button
                  onClick={submitQuizAnswer}
                  disabled={quizSelectedOption === null}
                  className="px-5 py-2 bg-orange-500 text-slate-950 rounded-lg text-xs font-bold disabled:opacity-50"
                >
                  تأكيد الإجابة
                </button>
              ) : (
                <div className="space-y-3 pt-2">
                  <div className={`p-3 rounded-lg text-xs border ${
                    quizSelectedOption === quizQuestions[quizIndex].correct
                      ? 'bg-emerald-500/10 border-emerald-500 text-emerald-300'
                      : 'bg-rose-500/10 border-rose-500 text-rose-300'
                  }`}>
                    {quizQuestions[quizIndex].explanation}
                  </div>
                  <button
                    onClick={nextQuizQuestion}
                    className="px-5 py-2 bg-slate-800 hover:bg-slate-700 text-slate-100 rounded-lg text-xs font-bold"
                  >
                    السؤال التالي
                  </button>
                </div>
              )}
            </div>
          </div>
        )}

      </main>

      {/* Footer */}
      <footer className="border-t border-slate-800 bg-slate-900/40 mt-12 py-4 text-center text-xs text-slate-500">
        منصة "مستكشف انتقال الحرارة" | Heat Transfer Explorer &copy; 2026 - صُممت خصيصاً لطلاب الميكانيكا والهندسة
      </footer>
    </div>
  );
}
