import { motion } from "framer-motion";

export default function Intro() {
  return (
    <main className="min-h-screen bg-black text-white flex flex-col items-center justify-center px-6 font-mono">
      {/* Typing intro */}
      <motion.h1
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 1 }}
        className="text-3xl md:text-4xl text-center mb-4"
      >
        👋 Hey there, I'm <span className="font-bold">Ansh</span>
      </motion.h1>

      {/* Subtitle */}
      <motion.h2
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 0.2, duration: 1 }}
        className="text-xl text-gray-300 mb-10 text-center"
      >
        Developer / Entrepreneur — Bringing imagination to life.
      </motion.h2>

      {/* About */}
      <motion.section
        initial={{ opacity: 0, y: 30 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 0.4, duration: 1 }}
        className="max-w-2xl text-sm text-gray-400 leading-relaxed space-y-3"
      >
        <p>
          🚀 Currently building <strong>Crypto-Tracker</strong> — an app that helps
          predict market surges and dips of major cryptocurrencies.
        </p>
        <p>
          💡 Worked on <strong>Stable Coin</strong>, <strong>E-commerce</strong>,{" "}
          <strong>Ticket Handler</strong>, and more.
        </p>
        <p>
          🧠 Learning <strong>Web3</strong>, <strong>AI</strong>, and <strong>ML</strong>{" "}
          while focusing on real-world applications.
        </p>
        <p>
          💻 Passionate about efficient systems, fluid UI, and perfecting dev setups.
        </p>
      </motion.section>

      {/* Tech Stack */}
      <motion.section
        initial={{ opacity: 0, y: 30 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 0.6, duration: 1 }}
        className="mt-10 max-w-2xl text-center"
      >
        <h3 className="text-lg font-semibold mb-3 text-white/90">⚙️ Tech Stack</h3>
        <p className="text-gray-400 text-sm leading-6">
          <strong>Languages:</strong> Rust · TypeScript · Lua · JSX · TSX  
          <br />
          <strong>Frameworks:</strong> Next.js · React · Tailwind CSS · Framer Motion  
          <br />
          <strong>Tools:</strong> Web3 · App Dev · APIs · Nvim (Packer + LazyVim) · VS Code
        </p>
      </motion.section>

      {/* Devices */}
      <motion.section
        initial={{ opacity: 0, y: 30 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 0.8, duration: 1 }}
        className="mt-10 text-center text-gray-400 text-sm"
      >
        <p>
          💻 MacBook M4 Pro · 🖱️ Logitech G304 Pro · ⌨️ Aula F87 Keyboard
        </p>
      </motion.section>

      {/* Hobbies */}
      <motion.section
        initial={{ opacity: 0, y: 30 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 1, duration: 1 }}
        className="mt-10 text-center text-gray-400 text-sm"
      >
        <h3 className="text-white/90 font-semibold mb-2">🎨 Hobbies</h3>
        <p>Customizing configs · Reading · Exploring design and digital art</p>
      </motion.section>

      {/* Footer animation line */}
      <motion.div
        initial={{ scaleX: 0 }}
        animate={{ scaleX: 1 }}
        transition={{ delay: 1.2, duration: 1.5, ease: "easeInOut" }}
        className="mt-12 w-40 h-[1px] bg-white/20 origin-left"
      />
    </main>
  );
}
