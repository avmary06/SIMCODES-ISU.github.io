# SIMCODES-ISU.github.io
Source for the SIMCODES website

## Building Locally

1. Ensure `ruby-bundler` is installed. On Ubuntu this is done by:

   ```.sh
   sudo apt install ruby-dev ruby-bundler
   ```

2. Clone this repo, i.e.,

   ```.sh
   git clone https://github.com/SIMCODES-ISU/SIMCODES-ISU.github.io
   ```

3. Install the dependencies via bundler. This is done by:

   ```.sh
   cd SIMCODES-ISU.github.io/docs
   bundle config set path 'vendor/bundle'
   bundle install
   ```

4. Launch the website server via:

   ```.sh
   bundle exec jekyll serve
   ```