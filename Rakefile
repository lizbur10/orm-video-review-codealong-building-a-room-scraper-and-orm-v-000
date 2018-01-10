require_relative './config/environment'

def reload!
    load_all './lib'
end

task :console do
    pry.start
end

task :scrape_rooms do
    boston_scraper = RoomScraper.new("https://boston.craigslist.org/search/roo")
    boston_scraper.call
    san_fran_scraper = RoomScraper.new("https://sfbay.craigslist.org/search/sfc/roo")
    san_fran_scraper.call
end