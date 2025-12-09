import React, { useState, useEffect } from 'react';
import { CheckCircle, XCircle, ChevronRight, ChevronLeft, RefreshCcw, BookOpen, Trophy, Award, List, ArrowLeft } from 'lucide-react';

const QuizApp = () => {
  const [currentQuestion, setCurrentQuestion] = useState(0);
  const [showScore, setShowScore] = useState(false);
  // เปลี่ยนการเก็บคะแนนและคำตอบ เป็น Array เพื่อให้ย้อนกลับไปมาได้
  const [userAnswers, setUserAnswers] = useState([]); 
  const [hasFinished, setHasFinished] = useState(false); // เช็คว่าเคยทำจบหรือยัง

  // ข้อมูลข้อสอบ 40 ข้อ
  const questions = [
    // --- บทที่ 8 ---
    {
      question: "ข้อใดอธิบายความหมายของ 'การแบ่งส่วนตลาด' (Market Segmentation) ได้ถูกต้องและชัดเจนที่สุด?",
      options: [
        "ก. บริษัทน้ำดื่ม A ผลิตน้ำดื่มบรรจุขวดแบบมาตรฐานเพียงแบบเดียว",
        "ข. แบรนด์เสื้อผ้า B จัดกลุ่มลูกค้าเป็น 'กลุ่มวัยรุ่นสตรีท' และ 'กลุ่มวัยทำงานเรียบหรู'",
        "ค. ร้านกาแฟ C เลือกเปิดสาขาเฉพาะในย่านสีลมและสาทร",
        "ง. บริษัทสมาร์ทโฟน D สร้างจุดขายว่ากล้องชัดที่สุดในโลก"
      ],
      correct: 1,
      explanation: "ข. ถูกต้อง เพราะการแบ่งส่วนตลาดคือการจัดกลุ่มผู้บริโภคที่มีความต้องการคล้ายกันออกจากกัน (ก=Mass Market, ค=Targeting, ง=Positioning)"
    },
    {
      question: "ข้อใด ไม่ใช่ เหตุผลหรือวัตถุประสงค์หลักของการทำ 'การแบ่งส่วนตลาด'?",
      options: [
        "ก. เพื่อให้ธุรกิจออกแบบผลิตภัณฑ์ตอบสนองลูกค้าได้แม่นยำขึ้น",
        "ข. เพื่อลดต้นทุนการผลิตให้ต่ำที่สุดโดยเน้นผลิตสินค้าแบบเดียว",
        "ค. เพื่อรักษาฐานลูกค้าเดิมโดยนำเสนอสิ่งที่ตรงใจ",
        "ง. เพื่อโฟกัสการสื่อสารและเลือกสื่อโฆษณาได้ตรงกลุ่ม"
      ],
      correct: 1,
      explanation: "ข. เป็นแนวคิดของ Mass Marketing (เน้นปริมาณมาก ต้นทุนต่ำ) ไม่ใช่ Segmentation"
    },
    {
      question: "สถานการณ์ใดสะท้อนถึง 'ประโยชน์ของการแบ่งส่วนตลาด' ในเรื่องการมองเห็นโอกาสทางการตลาดได้ชัดเจนที่สุด?",
      options: [
        "ก. บริษัทน้ำอัดลมทุ่มงบโฆษณาทีวีปูพรมทั่วประเทศ",
        "ข. แบรนด์เครื่องสำอางเห็นช่องว่าง 'ผู้ชายวัยทำงาน' ที่ต้องการครีมไม่เหนียว จึงออกสินค้าใหม่",
        "ค. ร้านสะดวกซื้อวางสินค้าเหมือนกันทุกสาขา",
        "ง. โรงงานผลิตเสื้อยืดสีขาว Free Size อย่างเดียว"
      ],
      correct: 1,
      explanation: "ข. ถูกต้อง เพราะการแบ่งส่วนตลาดทำให้เห็น 'ช่องว่าง' หรือ Niche Market ที่คู่แข่งยังทำไม่ถึง"
    },
    {
      question: "แบรนด์แชมพูแยกสูตร (ขจัดรังแค, ผมนุ่ม, ลดผมร่วง) เป็นการใช้เกณฑ์การแบ่งส่วนตลาดแบบใด?",
      options: [
        "ก. เกณฑ์ประชากรศาสตร์ (Demographic)",
        "ข. เกณฑ์จิตวิทยา (Psychographic)",
        "ค. เกณฑ์พฤติกรรม (Behavioristic)",
        "ง. เกณฑ์ภูมิศาสตร์ (Geographic)"
      ],
      correct: 2,
      explanation: "ค. ถูกต้อง (หัวข้อ Benefit Sought หรือผลประโยชน์ที่แสวงหา) ลูกค้าเลือกซื้อจากผลลัพธ์ที่ต้องการ"
    },
    {
      question: "ในกระบวนการ STP เมื่อทำ Segmentation (ขั้น 1-2) เสร็จแล้ว ขั้นตอนถัดไป (ขั้นที่ 3) คืออะไร?",
      options: [
        "ก. ตัดสินใจเลือกกลุ่มลูกค้าที่ดีที่สุดมาเป็นตลาดเป้าหมาย",
        "ข. ทำการประเมินความน่าสนใจและศักยภาพของแต่ละส่วนตลาด",
        "ค. สร้างจุดยืนและกำหนดตำแหน่งผลิตภัณฑ์",
        "ง. ออกแบบส่วนประสมทางการตลาด (4Ps)"
      ],
      correct: 1,
      explanation: "ข. ต้อง 'ประเมินความน่าสนใจ' (Evaluate) ก่อน แล้วค่อย 'เลือก' (Select) ในขั้นที่ 4"
    },
    {
      question: "โค้ก (Coke) ในอดีตผลิตรสชาติเดียว ขวดเดียว ขายทุกคนทั่วโลก จัดเป็นกลยุทธ์ใด?",
      options: [
        "ก. กลยุทธ์ตลาดหลายส่วน (Differentiated)",
        "ข. กลยุทธ์เฉพาะส่วนตลาด (Concentrated)",
        "ค. กลยุทธ์ตลาดรวม (Undifferentiated)",
        "ง. กลยุทธ์การตลาดจุลภาค (Micromarketing)"
      ],
      correct: 2,
      explanation: "ค. ตลาดรวม (Mass/Undifferentiated) มองลูกค้าทุกคนเหมือนกันหมด"
    },
    {
      question: "Honda ผลิตรถหลายรุ่น (City, Civic, Accord) เพื่อตอบโจทย์ลูกค้าต่างกลุ่มกัน ใช้กลยุทธ์ใด?",
      options: [
        "ก. กลยุทธ์ตลาดรวม",
        "ข. กลยุทธ์หลายส่วนตลาด ",
        "ค. กลยุทธ์เฉพาะส่วนตลาด",
        "ง. กลยุทธ์การตลาดส่วนบุคคล"
      ],
      correct: 1,
      explanation: "ข. หลายส่วนตลาด คือเลือกเป้าหมายมากกว่า 1 กลุ่ม และทำสินค้าต่างกันให้แต่ละกลุ่ม"
    },
    {
      question: "แชมพู Nizoral เน้นเจาะกลุ่มลูกค้าที่มีปัญหารังแค/เชื้อรา เพียงกลุ่มเดียว ใช้กลยุทธ์ใด?",
      options: [
        "ก. กลยุทธ์ตลาดรวม",
        "ข. กลยุทธ์หลายส่วนตลาด",
        "ค. กลยุทธ์เฉพาะส่วนตลาด ",
        "ง. กลยุทธ์การสร้างความแตกต่าง"
      ],
      correct: 2,
      explanation: "ค. เฉพาะส่วนตลาด (Niche/Concentrated) โฟกัสกลุ่มเล็กๆ กลุ่มเดียวที่ตนเชี่ยวชาญ"
    },
    {
      question: "Volvo สร้างภาพลักษณ์ว่าเป็น 'รถยนต์ที่ปลอดภัยที่สุด' เทียบกับคู่แข่ง ตรงกับข้อใด?",
      options: [
        "ก. การแบ่งส่วนตลาด",
        "ข. การเลือกตลาดเป้าหมาย",
        "ค. การกำหนดตำแหน่งผลิตภัณฑ์ ",
        "ง. การสร้างตราสินค้า"
      ],
      correct: 2,
      explanation: "ค. Positioning คือการปักธงในใจลูกค้าว่าเราคือใคร เด่นเรื่องอะไรเมื่อเทียบกับคู่แข่ง"
    },
    {
      question: "สิงคโปร์แอร์ไลน์ เด่นเรื่องความสุภาพและการบริการของพนักงานต้อนรับ เป็น Differentiation ด้านใด?",
      options: [
        "ก. ด้านผลิตภัณฑ์",
        "ข. ด้านภาพลักษณ์",
        "ค. ด้านช่องทางจัดจำหน่าย",
        "ง. ด้านบุคลากร "
      ],
      correct: 3,
      explanation: "ง. Personnel Differentiation คือความแตกต่างที่ตัวบุคคล/พนักงาน"
    },
    {
      question: "สมาร์ทโฟนจอพับ ยอดขายพุ่งเร็ว ลูกค้ายอมรับมากขึ้น คู่แข่งเริ่มเข้ามา แอยู่ในช่วงใดของ PLC?",
      options: [
        "ก. ขั้นแนะนำ (Introduction)",
        "ข. ขั้นเจริญเติบโต (Growth)",
        "ค. ขั้นอิ่มตัว (Maturity)",
        "ง. ขั้นถดถอย (Decline)"
      ],
      correct: 1,
      explanation: "ข. Growth Stage: ยอดขายโตเร็ว คู่แข่งรายใหม่เริ่มเข้ามา"
    },
    {
      question: "สินค้าเข้าสู่ 'ขั้นแนะนำ (Introduction)' ควรวางแผนโปรโมชั่นอย่างไร?",
      options: [
        "ก. ลดราคาทันทีเพื่อแย่งลูกค้า",
        "ข. โฆษณาแบบตอกย้ำ ",
        "ค. ทุ่มงบโฆษณาเพื่อสร้างการรับรู้ ",
        "ง. ตัดงบโฆษณาออก"
      ],
      correct: 2,
      explanation: "ค. ขั้นแนะนำต้องเน้นสร้าง Awareness ให้คนรู้จักและอยากลอง"
    },
    {
      question: "กราฟแกนตั้ง-แกนนอน (เช่น ราคา vs คุณภาพ) ที่ใช้ดูตำแหน่งแบรนด์เทียบคู่แข่ง เรียกว่าอะไร?",
      options: [
        "ก. SWOT Analysis",
        "ข. Positioning Map ",
        "ค. Marketing Mix Model",
        "ง. Product Life Cycle Graph"
      ],
      correct: 1,
      explanation: "ข. Perceptual Map หรือ Positioning Map ใช้แสดงตำแหน่งสินค้าในสายตาผู้บริโภค"
    },
    {
      question: "แบรนด์ Hermès เน้นขายความภาคภูมิใจและสถานะทางสังคม เป็นการวางตำแหน่งแบบใด?",
      options: [
        "ก. Functional Positioning",
        "ข. Emotional Positioning",
        "ค. Differentiation Positioning",
        "ง. Price Positioning"
      ],
      correct: 1,
      explanation: "ข. Emotional เน้นอารมณ์ความรู้สึก ภาพลักษณ์ มากกว่าฟังก์ชันการใช้งาน"
    },
    {
      question: "ข้อใดคือสโลแกนที่ 'ไม่ดี' (ทื่อ จำยาก ไม่น่าสนใจ) มากที่สุด?",
      options: [
        "ก. เป้าหมายมีไว้พุ่งชน",
        "ข. หอมกรุ่นจากเตาทุกวัน",
        "ค. เราคือผู้นำด้านการผลิตสินค้าอุปโภคบริโภคที่มีมาตรฐานสากล...",
        "ง. คิดจะดื่ม ดื่มคริสตัล"
      ],
      correct: 2,
      explanation: "ค. ยาวเกินไป ใช้คำทางการ จำยาก ขาดอารมณ์ร่วม (ไม่เข้าเกณฑ์สั้น กระชับ โดนใจ)"
    },
    {
      question: "ยาสีฟันสมุนไพร vs ยาสีฟันเจล ถือเป็นคู่แข่งกันเพราะเหตุผลใดสำคัญที่สุด?",
      options: [
        "ก. ราคาใกล้เคียงกัน",
        "ข. สนองความต้องการของลูกค้ากลุ่มเดียวกัน",
        "ค. ใช้พรีเซนเตอร์วัยรุ่นเหมือนกัน",
        "ง. ขายใน 7-Eleven เหมือนกัน"
      ],
      correct: 1,
      explanation: "ข. แนวคิดการแข่งขันมองที่ 'การตอบสนองความต้องการ' (Need) พื้นฐานเดียวกัน (ความสะอาดในช่องปาก)"
    },
    // --- หมวดที่ 1: บทที่ 11 ---
    {
      question: "ในมุมมอง 4Cs ส่วนผสม 'ราคา (Price)' ของธุรกิจ ตรงกับมุมมองลูกค้าในข้อใด?",
      options: [
        "ก. ความสะดวกสบาย (Convenience)",
        "ข. การสื่อสาร (Communication)",
        "ค. ต้นทุนของลูกค้า (Customer Cost)",
        "ง. การแก้ปัญหาให้ลูกค้า (Customer Solution)"
      ],
      correct: 2,
      explanation: "ค. Price = Cost to satisfy (ต้นทุนที่ลูกค้าต้องจ่าย ทั้งเงิน เวลา และความพยายาม)"
    },
    {
      question: "โรงแรมแถมบริการสปาฟรี อาหารเช้า รถรับส่ง จัดอยู่ในระดับผลิตภัณฑ์ใด?",
      options: [
        "ก. ผลิตภัณฑ์หลัก",
        "ข. ผลิตภัณฑ์ควบ ",
        "ค. ผลิตภัณฑ์พื้นฐาน",
        "ง. ผลิตภัณฑ์ที่คาดหวัง"
      ],
      correct: 1,
      explanation: "ข. Augmented Product คือส่วนเสริม/บริการพิเศษที่เพิ่มเข้ามาให้เหนือคู่แข่ง"
    },
    {
      question: "'โลงศพ' หรือ 'ประกันชีวิต' จัดเป็นสินค้าประเภทใด?",
      options: [
        "ก. สินค้าสะดวกซื้อ",
        "ข. สินค้าเลือกซื้อ",
        "ค. สินค้าเจาะจงซื้อ",
        "ง. สินค้าไม่แสวงซื้อ "
      ],
      correct: 3,
      explanation: "ง. Unsought Goods คือของที่คนไม่คิดจะซื้อ หรือไม่เห็นความจำเป็นจนกว่าจะถึงเวลา"
    },
    {
      question: "Apple ตั้งราคา iPhone รุ่นใหม่ไว้สูงมากเพื่อเจาะกลุ่มคนยอมจ่าย แล้วค่อยลดราคาลง เรียกว่า?",
      options: [
        "ก. Market-Penetration Pricing",
        "ข. Market-Skimming Pricing",
        "ค. Psychological Pricing",
        "ง. Going-rate Pricing"
      ],
      correct: 1,
      explanation: "ข. Skimming (ตักไขมัน/หัวกะทิ) ตั้งราคาสูงช่วงแรกเพื่อกอบโกยกำไรสูงสุดจากกลุ่ม Early Adopter"
    },
    {
      question: "โฆษณาหนักๆ ให้ลูกค้าอยากกินจนต้องเดินไปถามซื้อที่ร้านค้า เรียกว่ากลยุทธ์อะไร?",
      options: [
        "ก. กลยุทธ์ผลัก (Push Strategy)",
        "ข. กลยุทธ์ดึง (Pull Strategy)",
        "ค. การขายโดยพนักงาน",
        "ง. Trade Promotion"
      ],
      correct: 1,
      explanation: "ข. Pull Strategy คือดึงให้ลูกค้าวิ่งเข้าหาสินค้า (ผ่านการโฆษณาไปยังผู้บริโภคโดยตรง)"
    },
    // --- หมวดที่ 2: บทที่ 12 ---
    {
      question: "หัวใจสำคัญที่สุดของ 'การตลาดทางตรง (Direct Marketing)' คือสิ่งใด?",
      options: [
        "ก. พนักงานขายจำนวนมาก",
        "ข. งบโฆษณาสูง",
        "ค. ฐานข้อมูลลูกค้า ",
        "ง. หน้าร้านสาขาเยอะๆ"
      ],
      correct: 2,
      explanation: "ค. ต้องมี Database ที่แม่นยำเพื่อเจาะจงตัวบุคคลได้"
    },
    {
      question: "การเชื่อมโยงข้อมูลหน้าร้าน เว็บ แอป เข้าด้วยกันอย่างไร้รอยต่อ เรียกว่า?",
      options: [
        "ก. Multi-Level Marketing",
        "ข. Omni-Channel Marketing",
        "ค. Telemarketing",
        "ง. Mass Marketing"
      ],
      correct: 1,
      explanation: "ข. Omni-Channel คือการผสานทุกช่องทางให้เป็นหนึ่งเดียว"
    },
    {
      question: "ต้องการให้เว็บติดอันดับ Google แบบธรรมชาติ (ไม่เสียเงิน) ต้องทำสิ่งใด?",
      options: [
        "ก. SEO (Search Engine Optimization)",
        "ข. SEM (Search Engine Marketing)",
        "ค. Email Marketing",
        "ง. Affiliate Marketing"
      ],
      correct: 0,
      explanation: "ก. SEO คือการปรับแต่งเว็บให้ติดอันดับ Search ธรรมชาติ (Organic)"
    },
    {
      question: "การใช้ Chatbot, AI วิเคราะห์ข้อมูลลูกค้าแบบ Real-time อยู่ในยุคการตลาดใด?",
      options: [
        "ก. Marketing 1.0",
        "ข. Marketing 3.0",
        "ค. Marketing 4.0",
        "ง. Marketing 5.0"
      ],
      correct: 3,
      explanation: "ง. Marketing 5.0 = Technology for Humanity (Data-Driven + AI)"
    },
    {
      question: "ข้อแตกต่างระหว่าง 'ขายตรง' (Direct Selling) กับ 'การตลาดทางตรง' (Direct Marketing)?",
      options: [
        "ก. ขายตรงใช้พนักงานเผชิญหน้า / การตลาดทางตรงใช้สื่อไม่ต้องเจอหน้า",
        "ข. ขายตรงเน้นสินค้าอุตสาหกรรม / การตลาดทางตรงเน้นอุปโภคบริโภค",
        "ค. ขายตรงไม่ต้องมีสินค้า / การตลาดทางตรงต้องมี",
        "ง. ขายตรงผิดกฎหมาย / การตลาดทางตรงถูกกฎหมาย"
      ],
      correct: 0,
      explanation: "ก. ขายตรง (เช่น แอมเวย์) ใช้คนไปขาย / การตลาดทางตรง (เช่น แคตตาล็อก, อีเมล) ใช้สื่อ"
    },
    // --- หมวดที่ 3: บทที่ 13 ---
    {
      question: "SME ไทยส่งออกครั้งแรก ต้องการความเสี่ยงต่ำที่สุด ควรใช้วิธีใด?",
      options: [
        "ก. การส่งออกทางอ้อม (Indirect Exporting)",
        "ข. การให้สิทธิบัตร (Licensing)",
        "ค. การร่วมทุน (Joint Venture)",
        "ง. การลงทุนโดยตรง (Direct Investment)"
      ],
      correct: 0,
      explanation: "ก. ส่งออกทางอ้อม (ผ่านคนกลาง) เสี่ยงน้อยสุด ลงทุนน้อยสุด แต่กำไรก็น้อยสุด"
    },
    {
      question: "ต้องการ 'ควบคุมเบ็ดเสร็จ' และกำไรสูงสุดในระยะยาว (ยอมรับความเสี่ยงสูงสุด) ควรใช้วิธีใด?",
      options: [
        "ก. การส่งออก",
        "ข. การให้สิทธิแฟรนไชส์",
        "ค. การลงทุนโดยตรง ",
        "ง. การร่วมทุน"
      ],
      correct: 2,
      explanation: "ค. Direct Investment คือไปตั้งบริษัท/โรงงานเอง คุมเองหมด เสี่ยงเองหมด"
    },
    {
      question: "McDonald's เปลี่ยนจากเนื้อวัวเป็นไก่/แกะ ในอินเดีย เรียกว่ากลยุทธ์ใด?",
      options: [
        "ก. Straight Extension",
        "ข. Product Adaptation",
        "ค. Product Invention",
        "ง. Communication Adaptation"
      ],
      correct: 1,
      explanation: "ข. Product Adaptation ปรับปรุงสินค้าให้เข้ากับท้องถิ่น"
    },
    {
      question: "การขายสินค้าในต่างประเทศต่ำกว่าทุนหรือต่ำกว่าราคาในประเทศตัวเอง เพื่อกำจัดคู่แข่ง คือ?",
      options: [
        "ก. Transfer Pricing",
        "ข. Dumping ",
        "ค. Standard Pricing",
        "ง. Dual Pricing"
      ],
      correct: 1,
      explanation: "ข. Dumping หรือการทุ่มตลาด มักผิดกฎหมายการค้าระหว่างประเทศ"
    },
    {
      question: "ปัจจัยใดคือ 'ความเสี่ยงด้านการเมือง' ในธุรกิจระหว่างประเทศ?",
      options: [
        "ก. อัตราแลกเปลี่ยนผันผวน",
        "ข. รสนิยมผู้บริโภคเปลี่ยน",
        "ค. รัฐบาลยึดกิจการหรือเปลี่ยนนโยบายกีดกัน",
        "ง. คู่แข่งลดราคาสู้"
      ],
      correct: 2,
      explanation: "ค. การเมือง/กฎหมาย เช่น การยึดทรัพย์ (Expropriation) หรือกีดกันทางการค้า"
    },
    {
      question: "บริษัท A (ไทย) จับมือ บริษัท B (ญี่ปุ่น) ตั้งบริษัทใหม่ C ร่วมกัน คือรูปแบบใด?",
      options: [
        "ก. Licensing",
        "ข. Franchising",
        "ค. Joint Venture",
        "ง. Direct Exporting"
      ],
      correct: 2,
      explanation: "ค. Joint Venture (ร่วมทุน) คือสร้างกิจการใหม่ร่วมกัน"
    },
    {
      question: "7-Eleven ในไทย โดย CP All ได้รับสิทธิ์บริหารและใช้แบรนด์จากบริษัทแม่ คือรูปแบบใด?",
      options: [
        "ก. Licensing",
        "ข. Franchising",
        "ค. Contract Manufacturing",
        "ง. Turnkey Project"
      ],
      correct: 1,
      explanation: "ข. Franchising (แฟรนไชส์) ครอบคลุมทั้งแบรนด์ ระบบบริหาร และวิธีดำเนินงาน"
    },
    {
      question: "ข้อดีที่สุดของ 'กลยุทธ์มาตรฐานทั่วโลก (Standardized)' คือ?",
      options: [
        "ก. ตอบสนองท้องถิ่นได้ดีที่สุด",
        "ข. ลดต้นทุน ",
        "ค. หลีกเลี่ยงปัญหากฎหมาย",
        "ง. สร้างสัมพันธ์รัฐบาล"
      ],
      correct: 1,
      explanation: "ข. ผลิตเหมือนกัน โฆษณาเหมือนกัน ช่วยประหยัดต้นทุนมหาศาล"
    },
    {
      question: "ข้อใดสะท้อนอิทธิพลของ 'วัฒนธรรม' ต่อการตลาดระหว่างประเทศ?",
      options: [
        "ก. ภาษีนำเข้า",
        "ข. การเลือกสีและสัญลักษณ์ในบรรจุภัณฑ์",
        "ค. อัตราเงินเฟ้อ",
        "ง. ระบบขนส่ง"
      ],
      correct: 1,
      explanation: "ข. สี ความเชื่อ ภาษา เป็นเรื่องละเอียดอ่อนทางวัฒนธรรม"
    },
    // --- หมวดที่ 4: บทที่ 14 ---
    {
      question: "ขั้นตอนแรกสุดและสำคัญที่สุดของกระบวนการวิจัยตลาดคือ?",
      options: [
        "ก. การเก็บรวบรวมข้อมูล",
        "ข. การวิเคราะห์ข้อมูล",
        "ค. การกำหนดปัญหาและวัตถุประสงค์",
        "ง. การนำเสนอผลงาน"
      ],
      correct: 2,
      explanation: "ค. ถ้ากำหนดปัญหาผิด วิจัยไปก็เสียเปล่า (Garbage in, Garbage out)"
    },
    {
      question: "'ข้อมูลที่ผู้อื่นเก็บรวบรวมไว้แล้ว' เช่น สถิติจากรัฐบาล เรียกว่า?",
      options: [
        "ก. ข้อมูลปฐมภูมิ (Primary)",
        "ข. ข้อมูลทุติยภูมิ (Secondary)",
        "ค. ข้อมูลเชิงคุณภาพ",
        "ง. ข้อมูลเชิงปริมาณ"
      ],
      correct: 1,
      explanation: "ข. Secondary Data ข้อมูลมือสอง เอามาใช้ต่อได้เลย ประหยัดเวลา"
    },
    {
      question: "ต้องการทราบ 'ความคิดเห็นเชิงลึก/ความรู้สึก' ควรใช้วิธีใด?",
      options: [
        "ก. การสังเกต",
        "ข. การสัมภาษณ์กลุ่มย่อย ",
        "ค. การสำรวจทางโทรศัพท์",
        "ง. การทดลอง"
      ],
      correct: 1,
      explanation: "ข. Focus Group/Interview เหมาะกับการหาข้อมูลเชิงคุณภาพ (Qualitative)"
    },
    {
      question: "ข้อมูลยอดขาย สต็อกสินค้า บัญชี จัดเป็นข้อมูลระบบย่อยใดของ MIS?",
      options: [
        "ก. ระบบข้อมูลภายในกิจการ ",
        "ข. ระบบข่าวกรองการตลาด",
        "ค. ระบบวิจัยการตลาด",
        "ง. ระบบสนับสนุนการตัดสินใจ"
      ],
      correct: 0,
      explanation: "ก. Internal Records คือข้อมูลที่เกิดขึ้นจากการทำงานปกติในบริษัท"
    },
    {
      question: "ข้อใด 'ไม่ใช่' ประโยชน์โดยตรงของการวิจัยตลาด?",
      options: [
        "ก. ช่วยให้ทราบความต้องการลูกค้า",
        "ข. ช่วยลดความเสี่ยงในการตัดสินใจ",
        "ค. รับประกันว่าสินค้าจะขายดี 100%",
        "ง. ช่วยประเมินผลการตลาด"
      ],
      correct: 2,
      explanation: "ค. วิจัยช่วยลดความเสี่ยง แต่ 'การันตีผลลัพธ์ 100%' ไม่ได้ เพราะมีปัจจัยภายนอกที่คุมไม่ได้"
    }
  ];

  // เตรียม state เริ่มต้น (array ว่างเท่าจำนวนข้อ)
  useEffect(() => {
    setUserAnswers(Array(questions.length).fill(null));
  }, []);

  // คำนวณสถานะปัจจุบัน
  const currentAnswer = userAnswers[currentQuestion];
  const isAnswered = currentAnswer !== null && currentAnswer !== undefined;

  const handleAnswerOptionClick = (index) => {
    if (isAnswered) return; // ถ้าตอบแล้ว ห้ามเปลี่ยน
    
    const newAnswers = [...userAnswers];
    newAnswers[currentQuestion] = index;
    setUserAnswers(newAnswers);
  };

  const handleNextQuestion = () => {
    if (currentQuestion < questions.length - 1) {
      setCurrentQuestion(currentQuestion + 1);
    } else {
      setHasFinished(true); // มาร์คว่าทำจบแล้วครั้งหนึ่ง
      setShowScore(true);
    }
  };

  const handlePrevQuestion = () => {
    if (currentQuestion > 0) {
      setCurrentQuestion(currentQuestion - 1);
    }
  };

  const restartQuiz = () => {
    setUserAnswers(Array(questions.length).fill(null));
    setCurrentQuestion(0);
    setShowScore(false);
    setHasFinished(false);
  };

  const calculateScore = () => {
    return userAnswers.filter((ans, index) => ans === questions[index].correct).length;
  };

  const jumpToQuestion = (index) => {
    setCurrentQuestion(index);
    setShowScore(false);
  };

  // ดึงรายการข้อที่ผิด
  const getWrongQuestions = () => {
    return questions.map((q, index) => ({...q, index, userAnswer: userAnswers[index]}))
      .filter(q => q.userAnswer !== null && q.userAnswer !== q.correct);
  };

  const wrongQuestions = getWrongQuestions();

  return (
    <div className="flex flex-col items-center justify-center min-h-screen bg-slate-50 p-4 font-sans text-slate-800">
      <div className="w-full max-w-2xl bg-white rounded-2xl shadow-xl overflow-hidden border border-slate-200">
        
        {/* Header Section */}
        <div className="bg-indigo-600 p-6 text-white relative">
          <div className="flex items-center justify-between">
            <h1 className="text-xl md:text-2xl font-bold flex items-center gap-2">
              <BookOpen className="w-6 h-6" />
              แบบทดสอบวิชา การตลาด
            </h1>
            {!showScore && (
              <div className="flex items-center gap-2">
                 {hasFinished && (
                  <button 
                    onClick={() => setShowScore(true)}
                    className="text-xs bg-indigo-500 hover:bg-indigo-400 px-2 py-1 rounded text-white mr-2 transition-colors"
                  >
                    ดูคะแนน
                  </button>
                 )}
                <span className="text-sm font-medium bg-indigo-500 px-3 py-1 rounded-full whitespace-nowrap">
                  {currentQuestion + 1} / {questions.length}
                </span>
              </div>
            )}
          </div>
          <p className="text-indigo-100 mt-2 text-sm">ทบทวนแต่ละบท</p>
        </div>

        {showScore ? (
          // Score Screen
          <div className="p-8 space-y-6">
            <div className="text-center">
              <div className="w-24 h-24 bg-yellow-100 rounded-full flex items-center justify-center mx-auto mb-4 animate-bounce">
                <Trophy className="w-12 h-12 text-yellow-600" />
              </div>
              <h2 className="text-3xl font-bold text-slate-800">คะแนนรวมของคุณ</h2>
              <div className="text-6xl font-extrabold text-indigo-600 my-4">
                {calculateScore()} <span className="text-2xl text-slate-400 font-normal">/ {questions.length}</span>
              </div>
              <p className="text-slate-500 mb-6">
                {calculateScore() > 35 ? "สุดยอดมากครับน้องออมทรัพย์! เตรียม A ได้เลย!" : 
                 calculateScore() > 25 ? "ทำได้ดีครับ! ทบทวนจุดที่ผิดอีกนิดรับรองเป๊ะ" : "พยายามอีกนิดนะครับ ลองทบทวนข้อที่ผิดด้านล่างดูนะ"}
              </p>
              
              <button 
                onClick={restartQuiz}
                className="flex items-center justify-center gap-2 w-full py-4 bg-indigo-600 hover:bg-indigo-700 text-white rounded-xl font-bold transition-all shadow-lg active:scale-95 mb-8"
              >
                <RefreshCcw className="w-5 h-5" /> ทำแบบทดสอบใหม่
              </button>
            </div>

            {/* Wrong Answers Section */}
            {wrongQuestions.length > 0 && (
              <div className="border-t border-slate-200 pt-6">
                <h3 className="text-xl font-bold text-slate-700 mb-4 flex items-center gap-2">
                  <XCircle className="w-6 h-6 text-red-500" /> 
                  รายการข้อที่ตอบผิด ({wrongQuestions.length} ข้อ)
                </h3>
                <p className="text-sm text-slate-500 mb-4">คลิกที่รายการเพื่อดูเฉลยละเอียด</p>
                
                <div className="space-y-3">
                  {wrongQuestions.map((q) => (
                    <button 
                      key={q.index}
                      onClick={() => jumpToQuestion(q.index)}
                      className="w-full text-left p-4 bg-red-50 hover:bg-red-100 border border-red-100 rounded-xl transition-all flex items-start justify-between group"
                    >
                      <div>
                        <span className="text-xs font-bold text-red-500 bg-white px-2 py-0.5 rounded border border-red-200 mb-1 inline-block">
                          ข้อที่ {q.index + 1}
                        </span>
                        <p className="text-slate-700 font-medium line-clamp-2">{q.question}</p>
                      </div>
                      <ChevronRight className="w-5 h-5 text-red-300 group-hover:text-red-500 mt-2" />
                    </button>
                  ))}
                </div>
              </div>
            )}
          </div>
        ) : (
          // Quiz Screen
          <div className="p-6 pb-24 relative min-h-[500px]"> 
            {/* Added pb-24 for bottom nav space */}
            
            {/* Progress Bar */}
            <div className="w-full bg-slate-100 rounded-full h-2.5 mb-6">
              <div 
                className="bg-indigo-600 h-2.5 rounded-full transition-all duration-300" 
                style={{ width: `${((currentQuestion + 1) / questions.length) * 100}%` }}
              ></div>
            </div>

            {hasFinished && (
               <button 
                  onClick={() => setShowScore(true)}
                  className="mb-4 text-indigo-600 hover:text-indigo-800 flex items-center gap-1 text-sm font-medium"
                >
                  <ArrowLeft className="w-4 h-4" /> กลับไปหน้าสรุปคะแนน
               </button>
            )}

            {/* Question */}
            <h2 className="text-xl font-semibold mb-6 text-slate-800 leading-relaxed animate-fade-in">
              {questions[currentQuestion].question}
            </h2>

            {/* Options */}
            <div className="space-y-3">
              {questions[currentQuestion].options.map((option, index) => {
                let buttonStyle = "w-full text-left p-4 rounded-xl border-2 transition-all duration-200 font-medium ";
                
                if (isAnswered) {
                  if (index === questions[currentQuestion].correct) {
                    buttonStyle += "bg-green-50 border-green-500 text-green-700"; // Correct Answer
                  } else if (index === currentAnswer) {
                    buttonStyle += "bg-red-50 border-red-500 text-red-700"; // User's Wrong Answer
                  } else {
                    buttonStyle += "bg-slate-50 border-slate-100 text-slate-400 opacity-60"; // Others
                  }
                } else {
                  buttonStyle += "bg-white border-slate-200 hover:border-indigo-400 hover:bg-indigo-50 text-slate-600 cursor-pointer active:scale-[0.99]";
                }

                return (
                  <button 
                    key={index}
                    onClick={() => handleAnswerOptionClick(index)}
                    className={buttonStyle}
                    disabled={isAnswered}
                  >
                    <div className="flex items-start gap-3">
                      {isAnswered && index === questions[currentQuestion].correct && (
                        <CheckCircle className="w-5 h-5 text-green-500 mt-0.5 flex-shrink-0" />
                      )}
                      {isAnswered && index === currentAnswer && index !== questions[currentQuestion].correct && (
                        <XCircle className="w-5 h-5 text-red-500 mt-0.5 flex-shrink-0" />
                      )}
                      <span>{option}</span>
                    </div>
                  </button>
                );
              })}
            </div>

            {/* Explanation */}
            {isAnswered && (
              <div className="mt-6 animate-fade-in">
                <div className={`p-4 rounded-xl mb-6 border-l-4 ${currentAnswer === questions[currentQuestion].correct ? 'bg-green-50 border-green-500 text-green-800' : 'bg-red-50 border-red-500 text-red-800'}`}>
                  <h3 className="font-bold flex items-center gap-2 mb-1">
                    <Award className="w-4 h-4" />
                    คำอธิบาย:
                  </h3>
                  <p className="text-sm opacity-90">{questions[currentQuestion].explanation}</p>
                </div>
              </div>
            )}

            {/* Bottom Navigation */}
            <div className="absolute bottom-0 left-0 w-full p-4 bg-white border-t border-slate-100 flex gap-3">
               <button 
                  onClick={handlePrevQuestion}
                  disabled={currentQuestion === 0}
                  className={`flex-1 py-3 rounded-xl font-bold flex items-center justify-center gap-2 transition-all ${
                    currentQuestion === 0 
                      ? "bg-slate-100 text-slate-400 cursor-not-allowed" 
                      : "bg-white border-2 border-slate-200 text-slate-600 hover:bg-slate-50 hover:border-slate-300"
                  }`}
                >
                  <ChevronLeft className="w-5 h-5" /> ย้อนกลับ
                </button>

                <button 
                  onClick={handleNextQuestion}
                  className="flex-1 py-3 bg-indigo-600 hover:bg-indigo-700 text-white rounded-xl font-bold flex items-center justify-center gap-2 transition-all shadow-lg active:scale-95"
                >
                  {currentQuestion === questions.length - 1 ? "ดูผลคะแนน" : "ข้อต่อไป"} <ChevronRight className="w-5 h-5" />
                </button>
            </div>

          </div>
        )}
      </div>
    </div>
  );
};

export default QuizApp;
