# firecrawl.search
use function firecrawl.search

const Firecrawl = require('@mendable/firecrawl-js').default;

const firecrawl = new Firecrawl({ apiKey: "fc-******************" });


async function main() {
  const results = await firecrawl.search('quán phở gia lai', {
  limit: 5,
  // scrapeOptions: { formats: ['links'] }
  location: "Vietnam"
  });
  console.log(results);
}

main();
