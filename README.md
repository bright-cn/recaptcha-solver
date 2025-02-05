# reCaptcha CAPTCHA 解决方案  
[![Promo](https://github.com/bright-cn/Awesome-Web-Scraping/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner%20CN.png)](https://bright.cn)

轻松利用 Bright Data 的先进 CAPTCHA 解决技术绕过 reCaptcha CAPTCHA。通过机器学习算法、[自动化 IP 轮换](https://bright.cn/solutions/rotating-proxies)以及强大的代理基础设施，确保稳定且顺畅地访问目标网站。  
Bright Data 的 CAPTCHA Solver 是 [**Scraping Browser**](https://bright.cn/products/scraping-browser) 和 [**Web Unlocker API**](https://bright.cn/products/web-unlocker) 的内置功能，可完整应对最复杂的 CAPTCHA 挑战。

## 功能特色  
- **快速解决 CAPTCHA**：自动且高效地解决 reCaptcha CAPTCHA，准确度高。  
- **IP 轮换**：通过自动重试和动态 IP 调整来避免封禁。  
- **浏览器指纹**：模拟真实用户活动，绕过复杂的机器人检测。  
- **JavaScript 渲染**：处理 JavaScript 密集型网站的动态内容。  
- **全球地域覆盖**：精准解锁全球任意地区的内容。  
- **无缝集成**：可与 Puppeteer、Playwright、Selenium 等工具轻松集成。  
- **事件监控**：跟踪 CAPTCHA 解决事件，如检测、成功或失败。

## 为什么选择 reCaptcha CAPTCHA 解决方案  
### **全球 20,000+ 客户的信赖**  
Bright Data 的 CAPTCHA Solver 以无可匹敌的可靠性和性能而受到开发者、企业和各大机构的信赖。  

### **由顶级代理网络提供支持**  
拥有超过 1 亿个 IP 及先进的地域定位功能，Bright Data 的代理基础设施可提供顺畅且不中断的 CAPTCHA 处理流程。  

### **基于 AI 的 CAPTCHA 解决方案**  
我们使用先进的 AI 逻辑来自动检测、分析并解决 CAPTCHA，能够处理重试、指纹和请求头，从而绕过最严格的反机器人措施。  

### **为开发者而生**  
- 与 Puppeteer、Playwright 和 Selenium 无缝对接。  
- 可完全自定义 CAPTCHA 解题参数。  
- 自动重试和动态 IP 调整，保证数据采集不间断。  

> **专家提示 💡**  
>> 已经有现成的 CAPTCHA 解决方案？可结合我们的 [Puppeteer](https://bright.cn/integration/puppeteer)、[Playwright](https://bright.cn/integration/playwright) 和 [Selenium](https://bright.cn/integration/selenium) 代理，最大化减少 CAPTCHA 阻碍。

## 工作原理  
Bright Data 的 CAPTCHA Solver 集成在 **Scraping Browser** 和 **Web Unlocker** 中，让原本繁琐的 CAPTCHA 解决过程变得简洁高效。

### **自动化 CAPTCHA 解决**  
CAPTCHA Solver 会在实时环境中自动侦测并解决 CAPTCHA。只需启用功能，从检测到解题的每一步都可自动完成。  

#### 示例流程：  
1. **检测 CAPTCHA**：识别 CAPTCHA 类型（例如 reCaptcha）。  
2. **解决 CAPTCHA**：使用 AI 逻辑解决 CAPTCHA。  
3. **失败重试**：若解题失败，系统会自动切换到新 IP 并重试。  
4. **返回结果**：一旦成功解决，即可无缝访问目标网站。  

## 支持的 CAPTCHA 类型  
Bright Data 的 CAPTCHA Solver 支持多种不同的 CAPTCHA 类型，包括：  
- [**DataDome**](https://bright.cn/products/web-unlocker/captcha-solver/datadome)  
- [**reCAPTCHA**](https://bright.cn/products/web-unlocker/captcha-solver/recaptcha)  
- [**Click Captcha**](https://bright.cn/products/web-unlocker/captcha-solver/click-captcha)  
- [**hCaptcha**](https://bright.cn/products/web-unlocker/captcha-solver/hcaptcha)  
- [**PerimeterX**](https://brightdata.com/products/web-unlocker/captcha-solver/perimeterx)  
- [**SimpleCaptcha**](https://bright.cn/products/web-unlocker/captcha-solver/simplecaptcha)  
- [**FunCaptcha**](https://bright.cn/products/web-unlocker/captcha-solver/funcaptcha)  
- [**Cloudflare Turnstile**](https://brightdata.com/products/web-unlocker/captcha-solver/cloudflare-turnstile)  
- [**AWS WAF Captcha**](https://brightdata.com/products/web-unlocker/captcha-solver/aws-waf-captcha)  
- [**GeeTest CAPTCHA**](https://brightdata.com/products/web-unlocker/captcha-solver/geetest-captcha)  
- [**KeyCAPTCHA**](https://bright.cn/products/web-unlocker/captcha-solver/keycaptcha)  
- [**Puzzle CAPTCHA**](https://bright.cn/products/web-unlocker/captcha-solver/puzzle-captcha)  
- [**Yandex CAPTCHA**](https://bright.cn/products/web-unlocker/captcha-solver/yandex-captcha)  
- [**Image CAPTCHA**](https://brightdata.com/products/web-unlocker/captcha-solver/image-captcha)  
- [**Text CAPTCHA**](https://bright.cn/products/web-unlocker/captcha-solver/text-captcha)  

## 高级自定义  
[Bright Data 的 CAPTCHA Solver](https://github.com/luminati-io/Captcha-solver) 提供了高级自定义功能，可根据特定用途微调解题逻辑。

### **DataDome 挑战的自定义选项**  
```javascript
// Define default options for different CAPTCHA types
function getCaptchaOptions(captchaType, customOptions = {}) {
  const defaultOptions = {
    timeout: 30000, // Maximum time (in ms) to wait for CAPTCHA solving
    check_timeout: 500, // Interval (in ms) to check the CAPTCHA's status
    wait_networkidle: { timeout: 1000 }, // Wait until the network is idle for 1 second
    debug: false // Debug mode (disabled by default)
  };
  // Define CAPTCHA-specific selectors
  const captchaSelectors = {
    DataDome: { selector: '#datadome-captcha', success_selector: '#captcha-success' },
    reCAPTCHA: { selector: '.g-recaptcha', success_selector: '.recaptcha-success' },
    ClickCaptcha: { selector: '.click-captcha', success_selector: '.captcha-passed' },
    hCaptcha: { selector: '.h-captcha', success_selector: '.hcaptcha-success' },
    PerimeterX: { selector: '#px-captcha', success_selector: '#px-success' },
    SimpleCaptcha: { selector: '.simple-captcha', success_selector: '.captcha-done' },
    FunCaptcha: { selector: '.funcaptcha', success_selector: '.funcaptcha-success' },
    CloudflareTurnstile: { selector: '.cf-turnstile', success_selector: '.cf-success' },
    AWSWAF: { selector: '#aws-waf-captcha', success_selector: '#aws-waf-success' },
    GeeTest: { selector: '.geetest-captcha', success_selector: '.geetest-success' },
    KeyCAPTCHA: { selector: '#keycaptcha', success_selector: '#keycaptcha-success' },
    PuzzleCAPTCHA: { selector: '.puzzle-captcha', success_selector: '.puzzle-solved' },
    YandexCAPTCHA: { selector: '#yandex-captcha', success_selector: '#yandex-success' },
    ImageCAPTCHA: { selector: '.image-captcha', success_selector: '.image-captcha-success' },
    TextCAPTCHA: { selector: '.text-captcha', success_selector: '.text-captcha-success' }
  };
  // Get the correct selectors for the given CAPTCHA type
  const selectedOptions = captchaSelectors[captchaType] || {};
  // Merge default options with selected CAPTCHA-specific options and any custom overrides
  return { ...defaultOptions, ...selectedOptions, ...customOptions };
}
// Example usage for different CAPTCHA types
const ddOptions = getCaptchaOptions('DataDome', { timeout: 40000, debug: true });
const recaptchaOptions = getCaptchaOptions('reCAPTCHA', { debug: true });
const hcaptchaOptions = getCaptchaOptions('hCaptcha');
console.log(ddOptions);
console.log(recaptchaOptions);
console.log(hcaptchaOptions);
// Example error handling
try {
  if (!document.querySelector(ddOptions.selector)) {
    throw new Error(`CAPTCHA element not found using selector: ${ddOptions.selector}`);
  }
  // Your CAPTCHA-solving logic here
  solveCaptcha(ddOptions);
} catch (error) {
  console.error('Failed to solve CAPTCHA:', error.message);
}
```
## **事件监控**  
跟踪 CAPTCHA 解决事件，以处理高级用例：  
- `Captcha.detected`: 检测到 CAPTCHA 并开始解决。  
- `Captcha.solveFinished`: CAPTCHA 成功解决。  
- `Captcha.solveFailed`: CAPTCHA 解决失败。  

## **价格**  
| **方案**          | **价格（每 1K 结果）** | **月度费用**      | **描述**                                  |  
|-------------------|------------------------|------------------|-------------------------------------------|  
| **按需付费**      | $1.50                 | 无承诺           | 适合临时或零散的爬取需求。               |  
| **Growth**        | $1.27                 | $499             | 为扩展团队量身定制。                     |  
| **Business**      | $1.12                 | $999             | 适用于大规模爬取操作。                   |  
| **Premium**       | $1.05                 | $1,999           | 提供高级功能及优先支持。                 |  
| **Enterprise**    | 自定义报价            | 联系我们         | 针对顶级业务需求定制专属方案。           |  

🚀 **特别优惠**：首次充值可享受高达 **$500** 的等额赠送！  

## **为什么开发者钟爱 reCaptcha CAPTCHA 解决方案**  
- **简单集成**：与 Puppeteer、Playwright 和 Selenium 无缝兼容。  
- **先进的 AI 逻辑**：自动处理重试、CAPTCHA 解决、指纹、IP 轮换以及高级请求头。  
- **内置浏览器**：无需管理外部浏览器来进行 JavaScript 渲染。  
- **实时洞察**：通过实时仪表板监控网络性能。  
- **无与伦比的支持**：24/7 全球客户支持，并持续推出新功能。  

## **常见问题**  
### **reCaptcha CAPTCHA 解决方案如何工作？**  
该解决方案使用先进的基于 AI 的逻辑，自动检测并解决 reCaptcha CAPTCHA。  

### **它能同时处理多个 CAPTCHA 吗？**  
可以。该解决方案可扩展以同时处理多种 CAPTCHA 类型，确保访问不中断。  

### **如果 CAPTCHA 解决失败会怎样？**  
系统会自动重试。如果问题仍然存在，请联系我们的 24/7 支持团队进行排查。  

---  

## **告别 reCaptcha CAPTCHA 的烦恼**  
立即开始免费试用，体验 Bright Data 带来的无缝 [reCaptcha CAPTCHA 解决方案](https://bright.cn/products/web-unlocker/captcha-solver/recaptcha)！
