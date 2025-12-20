# ROI Calculator for TheHireHub.AI

A fully functional, intuitive ROI calculator that demonstrates cost savings when using TheHireHub.AI compared to traditional search firms and other AI recruitment tools. The calculator intelligently recommends the best pricing plan based on your hiring needs.

## Features

- **Dual Input Controls**: 
  - Number of hires per month (1-200)
  - Active job openings per month (1-50)
  
- **Intelligent Plan Recommendation**: 
  - Automatically suggests the best pricing plan (Startup, Early Stage, Growth, or Enterprise)
  - Shows plan features and pricing
  - Updates in real-time as you adjust inputs

- **Real-time Calculations**: 
  - Total leads to be reached
  - Leads assessed & qualified
  - Total selections
  - Job slots needed

- **Detailed Cost Comparison**: 
  - Monthly cost breakdown (Without vs With TheHireHub.AI)
  - Annual savings calculation
  - Cost breakdown showing traditional search firm fees vs platform cost

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices

- **Indian Numbering System**: Displays numbers and currency in Indian format (₹)

## Pricing Plans

The calculator uses your actual pricing plans:

1. **Startup Plan**: $99/month - 3 job slots
2. **Early Stage Plan**: $299/month - 10 job slots  
3. **Growth Plan**: $899/month - 25 job slots
4. **Enterprise Plan**: Custom pricing - Unlimited job slots

## How to Use

1. Open `roi-calculator.html` in any modern web browser
2. Adjust the sliders or input fields:
   - **No. of hires / month**: Set your monthly hiring target
   - **Active job openings / month**: Set concurrent positions you're hiring for
3. View the recommended plan and its features
4. See calculated metrics and cost comparisons
5. Review annual savings

## Calculation Logic

### Metrics
- **Leads per hire**: 103.7 (industry average)
- **Qualified leads per hire**: 13.6
- **Selections per hire**: 1.43 (accounting for ~70% offer acceptance)

### Cost Calculations
- **Traditional method**: ₹24,540 per hire (includes search firm fees 15-25% of salary + recruiter overhead)
- **TheHireHub.AI**: Based on recommended plan pricing converted to INR

### Plan Selection
The calculator automatically selects the plan based on job slots needed:
- 1-3 jobs → Startup Plan
- 4-10 jobs → Early Stage Plan
- 11-25 jobs → Growth Plan
- 26+ jobs → Enterprise Plan

## Customization

You can adjust the calculation metrics in the JavaScript section:

```javascript
// USD to INR conversion rate
const USD_TO_INR = 83;

// Industry metrics
const METRICS = {
    LEADS_PER_HIRE: 103.696,
    QUALIFIED_PER_HIRE: 13.61,
    SELECTIONS_PER_HIRE: 1.429,
    COST_PER_HIRE_TRADITIONAL: 24540,
};

// Pricing plans
const PLANS = {
    startup: {
        name: "Startup",
        monthlyPrice: 99,
        jobSlots: 3,
        // ... features
    },
    // ... other plans
};
```

## Integration

To integrate this calculator into your website:

1. Copy the HTML, CSS, and JavaScript into your existing page
2. Adjust the styling to match your brand colors (currently uses blue #2563eb)
3. Update the USD to INR conversion rate if needed
4. Customize the "Request a detailed custom quote" link to point to your contact form
5. Adjust cost metrics if your pricing changes

## Browser Support

Works on all modern browsers:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Notes

- The calculator is optimized for small to medium-scale hiring (1-200 hires/month)
- Costs are calculated in Indian Rupees (₹) with USD pricing converted at current rates
- All numbers are formatted using Indian numbering system (e.g., 5,18,480)
- Plan recommendations are based on job slots, not number of hires
- Enterprise plan shows estimated pricing (custom quote recommended)