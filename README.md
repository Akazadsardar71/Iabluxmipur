export default function HomePage() {
  return (
    <div className="min-h-screen bg-gray-100 text-gray-800">
      {/* Navigation */}
      <nav className="bg-green-800 text-white p-4 flex justify-between items-center shadow-md">
        <h1 className="text-2xl font-bold">ইসলামী আন্দোলন বাংলাদেশ</h1>
        <ul className="flex gap-4">
          <li><a href="#" className="hover:underline">হোম</a></li>
          <li><a href="#" className="hover:underline">আমাদের সম্পর্কে</a></li>
          <li><a href="#" className="hover:underline">নেতা ও কমিটি</a></li>
          <li><a href="#" className="hover:underline">কর্মসূচি</a></li>
          <li><a href="#" className="hover:underline">সংবাদ</a></li>
          <li><a href="#" className="hover:underline">মিডিয়া</a></li>
          <li><a href="#member-form" className="hover:underline">যোগাযোগ</a></li>
        </ul>
      </nav>

      {/* Hero Section */}
      <header className="bg-white text-center py-20 shadow-inner">
        <h2 className="text-4xl font-semibold mb-4">সত্য, ন্যায় ও ইসলামের পথে</h2>
        <p className="text-lg">ইসলামী আন্দোলন বাংলাদেশ একটি আদর্শিক রাজনৈতিক দল</p>
      </header>

      {/* Intro Section */}
      <section className="p-8 bg-gray-50">
        <div className="max-w-3xl mx-auto">
          <h3 className="text-2xl font-bold mb-4">আমাদের উদ্দেশ্য</h3>
          <p>
            ইসলামী আন্দোলন বাংলাদেশ একটি ইসলামী আদর্শ ভিত্তিক রাজনৈতিক সংগঠন যা দেশের কল্যাণ, ন্যায়বিচার, এবং ইসলামী মূল্যবোধ প্রতিষ্ঠার লক্ষ্যে কাজ করে যাচ্ছে। আমরা চাই একটি শান্তিপূর্ণ, সুশাসনময়, এবং ইসলামী রাষ্ট্রব্যবস্থা।
          </p>
        </div>
      </section>

      {/* Member Form Section */}
      <section id="member-form" className="p-8 bg-white">
        <div className="max-w-3xl mx-auto">
          <h3 className="text-2xl font-bold mb-6">কমিটির সদস্য ফরম</h3>
          <form className="grid grid-cols-1 gap-4">
            <input type="text" placeholder="পূর্ণ নাম" className="p-2 border rounded" required />
            <input type="text" placeholder="পিতার নাম" className="p-2 border rounded" required />
            <input type="text" placeholder="জাতীয় পরিচয়পত্র নম্বর" className="p-2 border rounded" required />
            <input type="date" className="p-2 border rounded" required />
            <input type="text" placeholder="ঠিকানা" className="p-2 border rounded" required />
            <select className="p-2 border rounded" required>
              <option value="">ওয়ার্ড নম্বর নির্বাচন করুন</option>
              {[...Array(9)].map((_, i) => (
                <option key={i + 1} value={i + 1}>{i + 1}</option>
              ))}
            </select>
            <input type="tel" placeholder="মোবাইল নম্বর" className="p-2 border rounded" required />
            <input type="email" placeholder="ইমেইল (ঐচ্ছিক)" className="p-2 border rounded" />
            <input type="text" placeholder="পেশা" className="p-2 border rounded" required />
            <input type="text" placeholder="শিক্ষাগত যোগ্যতা" className
